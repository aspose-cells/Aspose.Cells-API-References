##SparklineGroupCollection Class
'SparklineGroupCollection class. Encapsulates the object that represents sparklinegroupcollection in Go.'
## SparklineGroupCollection class
Encapsulates a collection of <see cref="SparklineGroup"/> objects.
```go
type SparklineGroupCollection struct  {
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
|[Get](./get/) | Gets the SparklineGroup element at the specified index. |
|[Add_SparklineType](./add_sparklinetype/) | Adds an SparklineGroup with a Sparkline to the collection. |
|[Add_SparklineType_String_Bool_CellArea](./add_sparklinetype_string_bool_cellarea/) | Adds an SparklineGroup with Sparkline to the collection. |
|[ClearSparklines](./clearsparklines/) | Clears the sparklines that is inside an area of cells. |
|[ClearSparklineGroups](./clearsparklinegroups/) | Clears the sparkline groups that overlaps an area of cells. |
|[GetCount](./getcount/) |  |
