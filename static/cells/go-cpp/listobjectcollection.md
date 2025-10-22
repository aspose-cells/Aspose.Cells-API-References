##ListObjectCollection Class
'ListObjectCollection class. Encapsulates the object that represents listobjectcollection in Go.'
## ListObjectCollection class
Represents a collection of <see cref="ListObject"/> objects in the worksheet.
```go
type ListObjectCollection struct  {
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
|[Get_Int](./get_int/) | Gets the ListObject by index. |
|[Get_String](./get_string/) | Gets the ListObject by specified name. |
|[Add_Int_Int_Int_Int_Bool](./add_int_int_int_int_bool/) | Adds a ListObject to the worksheet. |
|[Add_String_String_Bool](./add_string_string_bool/) | Adds a ListObject to the worksheet. |
|[UpdateColumnName](./updatecolumnname/) | Update all column name of the tables. |
|[GetCount](./getcount/) |  |
