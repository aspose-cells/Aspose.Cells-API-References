##TimelineCollection Class
'TimelineCollection class. Encapsulates the object that represents timelinecollection in Go.'
## TimelineCollection class
Specifies the collection of all the Timeline objects on the specified worksheet.Due to MS Excel, Excel 2003 does not support Timeline.
```go
type TimelineCollection struct  {
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
|[Get_Int](./get_int/) | Gets the Timeline by index. |
|[Get_String](./get_string/) | Gets the Timeline  by Timeline's name. |
|[Add_PivotTable_Int_Int_String](./add_pivottable_int_int_string/) | Add a new Timeline using PivotTable as data source |
|[Add_PivotTable_String_String](./add_pivottable_string_string/) | Add a new Timeline using PivotTable as data source |
|[Add_PivotTable_Int_Int_Int](./add_pivottable_int_int_int/) | Add a new Timeline using PivotTable as data source |
|[Add_PivotTable_String_Int](./add_pivottable_string_int/) | Add a new Timeline using PivotTable as data source |
|[Add_PivotTable_Int_Int_PivotField](./add_pivottable_int_int_pivotfield/) | Add a new Timeline using PivotTable as data source |
|[Add_PivotTable_String_PivotField](./add_pivottable_string_pivotfield/) | Add a new Timeline using PivotTable as data source |
|[GetCount](./getcount/) |  |
