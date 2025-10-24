##SlicerCollection Class
'SlicerCollection class. Encapsulates the object that represents slicercollection in Go.'
## SlicerCollection class
Specifies the collection of all the Slicer objects on the specified worksheet.
```go
type SlicerCollection struct  {
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
|[Get_Int](./get_int/) | Gets the Slicer by index. |
|[Get_String](./get_string/) | Gets the Slicer  by slicer's name. |
|[Remove](./remove/) | Remove the specified Slicer |
|[RemoveAt](./removeat/) | Deletes the Slicer at the specified index |
|[Clear](./clear/) | Clear all Slicers. |
|[Add_PivotTable_String_String](./add_pivottable_string_string/) | Add a new Slicer using PivotTable as data source |
|[Add_PivotTable_Int_Int_String](./add_pivottable_int_int_string/) | Add a new Slicer using PivotTable as data source |
|[Add_PivotTable_Int_Int_Int](./add_pivottable_int_int_int/) | Add a new Slicer using PivotTable as data source |
|[Add_PivotTable_String_Int](./add_pivottable_string_int/) | Add a new Slicer using PivotTable as data source |
|[Add_PivotTable_Int_Int_PivotField](./add_pivottable_int_int_pivotfield/) | Add a new Slicer using PivotTable as data source |
|[Add_PivotTable_String_PivotField](./add_pivottable_string_pivotfield/) | Add a new Slicer using PivotTable as data source |
|[Add_ListObject_Int_String](./add_listobject_int_string/) | Add a new Slicer using ListObjet as data source |
|[Add_ListObject_ListColumn_String](./add_listobject_listcolumn_string/) | Add a new Slicer using ListObjet as data source |
|[Add_ListObject_ListColumn_Int_Int](./add_listobject_listcolumn_int_int/) | Add a new Slicer using ListObjet as data source |
|[GetCount](./getcount/) |  |
