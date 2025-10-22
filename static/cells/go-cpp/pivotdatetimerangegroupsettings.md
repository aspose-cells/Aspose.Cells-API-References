##PivotDateTimeRangeGroupSettings Class
'PivotDateTimeRangeGroupSettings class. Encapsulates the object that represents pivotdatetimerangegroupsettings in Go.'
## PivotDateTimeRangeGroupSettings class
Represents the field grouped by date time range.
```go
type PivotDateTimeRangeGroupSettings struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewPivotDateTimeRangeGroupSettings](./newpivotdatetimerangegroupsettings/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetType](./gettype/) | Gets the data time group type. |
|[GetStart](./getstart/) | Gets the start date time of the group. |
|[GetEnd](./getend/) | Gets the end date time of the group. |
|[GetInterval](./getinterval/) | Gets the internal of the group. |
|[GetGroupByTypes](./getgroupbytypes/) | Gets the types of grouping by date time. |
|[IsGroupedBy](./isgroupedby/) | Check whether the field is grouped by the type. |
