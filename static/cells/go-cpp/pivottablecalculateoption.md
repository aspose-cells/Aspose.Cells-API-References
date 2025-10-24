##PivotTableCalculateOption Class
'PivotTableCalculateOption class. Encapsulates the object that represents pivottablecalculateoption in Go.'
## PivotTableCalculateOption class
Rerepsents the options of calcuating the pivot table.
```go
type PivotTableCalculateOption struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewPivotTableCalculateOption](./newpivottablecalculateoption/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetRefreshData](./getrefreshdata/) | Indicates whether refreshing data source of the pivottable. |
|[SetRefreshData](./setrefreshdata/) | Indicates whether refreshing data source of the pivottable. |
|[GetRefreshCharts](./getrefreshcharts/) | Indicates whether refreshing charts are based on this pivot table. |
|[SetRefreshCharts](./setrefreshcharts/) | Indicates whether refreshing charts are based on this pivot table. |
|[GetReserveMissingPivotItemType](./getreservemissingpivotitemtype/) | Represents how to reserve missing pivot items. |
|[SetReserveMissingPivotItemType](./setreservemissingpivotitemtype/) | Represents how to reserve missing pivot items. |
