##OleObjectCollection Class
'OleObjectCollection class. Encapsulates the object that represents oleobjectcollection in Go.'
## OleObjectCollection class
Represents embedded OLE objects.
```go
type OleObjectCollection struct  {
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
|[Add_Int_Int_Int_Int_Stream](./add_int_int_int_int_stream/) | Adds an OleObject to the collection. |
|[Add_Int_Int_Int_Int_Stream_String](./add_int_int_int_int_stream_string/) | Adds a linked OleObject to the collection. |
|[Get](./get/) | Gets the OleObject element at the specified index. |
|[Clear](./clear/) | Remove all embedded OLE objects. |
|[RemoveAt](./removeat/) | Removes the element at the specified index. |
|[GetCount](./getcount/) |  |
