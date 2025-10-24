##DocumentPropertyCollection Class
'DocumentPropertyCollection class. Encapsulates the object that represents documentpropertycollection in Go.'
## DocumentPropertyCollection class
Base class for <see cref="BuiltInDocumentPropertyCollection"/> and <see cref="CustomDocumentPropertyCollection"/> collections.
```go
type DocumentPropertyCollection struct  {
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
|[Get_Int](./get_int/) | Returns a DocumentProperty object by index. |
|[Contains](./contains/) | Returns true if a property with the specified name exists in the collection. |
|[IndexOf](./indexof/) | Gets the index of a property by name. |
|[Remove](./remove/) | Removes a property with the specified name from the collection. |
|[RemoveAt](./removeat/) | Removes a property at the specified index. |
|[Get_String](./get_string/) | Returns a DocumentProperty object by the name of the property. |
|[GetCount](./getcount/) |  |
