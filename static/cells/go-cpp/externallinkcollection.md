##ExternalLinkCollection Class
'ExternalLinkCollection class. Encapsulates the object that represents externallinkcollection in Go.'
## ExternalLinkCollection class
Represents external links collection in a workbook.
```go
type ExternalLinkCollection struct  {
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
|[GetCount](./getcount/) | Gets the number of elements actually contained in the collection. |
|[Add_String_stringArray](./add_string_stringarray/) | Adds an external link. |
|[Add_DirectoryType_String_stringArray](./add_directorytype_string_stringarray/) | Add an external link . |
|[Get](./get/) | Gets the ExternalLink element at the specified index. |
|[Clear](./clear/) | Removes all external links. |
|[Clear_Bool](./clear_bool/) | Removes all external links. |
|[RemoveAt_Int](./removeat_int/) | Removes the specified external link from the workbook. |
|[RemoveAt_Int_Bool](./removeat_int_bool/) | Removes the specified external link from the workbook. |
|[GetEnumerator](./getenumerator/) | Get an enumerator that iterates through this collection. |
