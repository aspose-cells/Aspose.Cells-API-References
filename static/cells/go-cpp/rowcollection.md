##RowCollection Class
'RowCollection class. Encapsulates the object that represents rowcollection in Go.'
## RowCollection class
Collects the <see cref="Row"/> objects that represent the individual rows in a worksheet.
```go
type RowCollection struct  {
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
|[GetCount](./getcount/) | Gets the number of rows in this collection. |
|[GetEnumerator](./getenumerator/) | Gets an enumerator that iterates rows through this collection |
|[GetEnumerator_Bool_Bool](./getenumerator_bool_bool/) | Gets an enumerator that iterates rows through this collection |
|[GetRowByIndex](./getrowbyindex/) | Gets the row object by the position in the list. |
|[Get](./get/) | Gets a Row object by given row index. The Row object of given row index will be instantiated if it does not exist before. |
|[Clear](./clear/) | Clear all rows and cells. |
|[RemoveAt](./removeat/) | Remove the row item at the specified index(position) in this collection. |
