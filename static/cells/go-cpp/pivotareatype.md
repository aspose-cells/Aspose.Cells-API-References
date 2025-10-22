##PivotAreaType Enum
'PivotAreaType enum. Encapsulates the object that represents pivotareatype in Go.'
## PivotAreaType Enum
Indicates the type of rule being used to describe an area or aspect of the PivotTable.
```go
type PivotAreaType int32
```
## Fields
| Field | Description |
| --- | --- |
|[None](./none/) | No Pivot area. |
|[Normal](./normal/) | Represents a header or item. |
|[Data](./data/) | Represents something in the data area. |
|[All](./all/) | Represents the whole PivotTable. |
|[Origin](./origin/) | Represents the blank cells at the top-left of the PivotTable (top-right for RTL sheets). |
|[Button](./button/) | Represents a field button. |
|[TopRight](./topright/) | Represents the blank cells at the top-right of the PivotTable (top-left for RTL sheets). |
