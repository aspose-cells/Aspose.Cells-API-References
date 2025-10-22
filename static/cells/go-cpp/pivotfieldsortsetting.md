##PivotFieldSortSetting Class
'PivotFieldSortSetting class. Encapsulates the object that represents pivotfieldsortsetting in Go.'
## PivotFieldSortSetting class
Represents the setting of sorting pivot fields.
```go
type PivotFieldSortSetting struct  {
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
|[GetSortType](./getsorttype/) | Represents the SortOrder. |
|[IsSortByLabels](./issortbylabels/) | Indicates whether sorting the field by itself or data field. |
|[GetFieldIndex](./getfieldindex/) | Represents the index of the field sorted by.-1 means sorting the PivotField by the labels,others means sorting by the data field. |
|[GetLineTypeSortedBy](./getlinetypesortedby/) | The pivot line type sorted by. |
|[IsSimpleSort](./issimplesort/) | Indicates whether a simple data sort operation will be applied. |
|[GetCell](./getcell/) | Sorts by the values in which row or column. |
