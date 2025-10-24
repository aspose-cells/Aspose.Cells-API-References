##ChartCollection Class
'ChartCollection class. Encapsulates the object that represents chartcollection in Go.'
## ChartCollection class
Encapsulates a collection of <see cref="Chart"/> objects.
```go
type ChartCollection struct  {
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
|[AddFloatingChart](./addfloatingchart/) | Adds a chart to the collection. |
|[Add_ChartType_Int_Int_Int_Int](./add_charttype_int_int_int_int/) | Adds a chart to the collection. |
|[Add_Stream_String_Bool_Int_Int_Int_Int](./add_stream_string_bool_int_int_int_int/) | Adds a chart with preset template. |
|[Add_ChartType_String_Bool_Int_Int_Int_Int](./add_charttype_string_bool_int_int_int_int/) | Adds a chart to the collection. |
|[Get_Int](./get_int/) | Gets the Chart element at the specified index. |
|[Get_String](./get_string/) | Gets the chart by the name. |
|[RemoveAt](./removeat/) | Remove a chart at the specific index. |
|[Clear](./clear/) | Clear all charts. |
|[GetCount](./getcount/) |  |
