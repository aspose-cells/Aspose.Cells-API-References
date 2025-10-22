##PivotItemCollection Class
'PivotItemCollection class. Encapsulates the object that represents pivotitemcollection in Go.'
## PivotItemCollection class
Represents all the <see cref="PivotItem"/> objects in the PivotField.
```go
type PivotItemCollection struct  {
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
|[GetEnumerator](./getenumerator/) | Gets an enumerator over the elements in this collection in proper sequence. |
|[Get_Int](./get_int/) | Gets the PivotItem Object at the specific index. |
|[Get_String](./get_string/) | Gets the PivotItem by the specific name. |
|[GetCount](./getcount/) | Gets the count of the pivot items. |
|[SwapItem](./swapitem/) | Directly swap two items. |
