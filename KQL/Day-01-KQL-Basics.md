# Day 1 - KQL fundamental

## Date
05-06-2026

## Topics Learned
- where
- project
- search
- contains

## Queries Practiced

```kql
AppAvailabilityResults
| where Location == "East US"
```

```kql
AppAvailabilityResults
| project Location
```

## Mistakes I Made
- Used search after table name
- Confused column and table names

## Key Takeaways
- search works on tables
- where filters columns

## Next Topic
- summarize
- let statement