##PivotTableSourceType Enum
'PivotTableSourceType enum. Encapsulates the object that represents pivottablesourcetype in Go.'
## PivotTableSourceType Enum
Represents data source type of the pivot table.
```go
type PivotTableSourceType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Sheet](./sheet/) | Specifies that the source data is a range. |
|[External](./external/) | Specifies that external source data is used. |
|[Consolidation](./consolidation/) | Specifies that multiple consolidation ranges are used as the source data. |
|[Scenario](./scenario/) | The source data is populated from a temporary internal structure. |
|[Unknown](./unknown/) | Unknown data source. |
