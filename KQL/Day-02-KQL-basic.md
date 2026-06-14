# Day 2 - KQL Joins and Geospatial Basics

## Date
14-06-2026

## Topics Learned
- lookup operator
- join operator
- inner join
- distinct
- query-generated tables
- render
- scatterchart
- kind=map
- geo_point_in_polygon
- geo_distance_point_to_line

## Queries Practiced

```kql
StormEvents
| where EventType == "Lightning"
| distinct State
```

```kql
StormEvents
| where EventType == "Lightning"
| distinct State
| join kind=inner (
    StormEvents
    | where EventType == "Avalanche"
    | distinct State
) on State
| project State
```

```kql
StormEvents
| take 100
| project BeginLon, BeginLat
| render scatterchart with (kind=map)
```

```kql
StormEvents
| take 100
| project BeginLon, BeginLat, EventType
| render scatterchart with (kind=map)
```

## Mistakes I Made

- Thought `lookup` and `join` were exactly the same.
- Forgot to use `distinct` before comparing states.
- Initially confused how `render` displays map data.

## Key Takeaways

- `lookup` is best for enriching a large table with data from a small table.
- `join` combines rows from two tables based on matching columns.
- `inner join` returns only matching records.
- `distinct` removes duplicate values.
- `render scatterchart with (kind=map)` plots latitude and longitude on a map.
- Geospatial functions (`geo_*`) are useful but lower priority for SC-200 compared to core KQL operators.

## Next Topic

- summarize
- count() and dcount()
- let statement
- union
- extend
- parse