##SubtotalSetting Class
'SubtotalSetting class. Encapsulates the object that represents subtotalsetting in Go.'
## SubtotalSetting class
Represents the setting of the subtotal .
```go
type SubtotalSetting struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetGroupBy](./getgroupby/) | The field to group by, as a zero-based integer offset |
|[GetSubtotalFunction](./getsubtotalfunction/) | The subtotal function. |
|[GetTotalList](./gettotallist/) | An array of zero-based field offsets, indicating the fields to which the subtotals are added. |
|[GetSummaryBelowData](./getsummarybelowdata/) | Indicates whether add summary below data. |
