##CustomDocumentPropertyCollection Class
'CustomDocumentPropertyCollection class. Encapsulates the object that represents customdocumentpropertycollection in Go.'
## CustomDocumentPropertyCollection class
A collection of custom document properties.
```go
type CustomDocumentPropertyCollection struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewCustomDocumentPropertyCollection](./newcustomdocumentpropertycollection/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[Add_String_String](./add_string_string/) | Creates a new custom document property of the <b>PropertyType.String</b> data type. |
|[Add_String_Int](./add_string_int/) | Creates a new custom document property of the <b>PropertyType.Number</b> data type. |
|[Add_String_Date](./add_string_date/) | Creates a new custom document property of the <b>PropertyType.DateTime</b> data type. |
|[Add_String_Bool](./add_string_bool/) | Creates a new custom document property of the <b>PropertyType.Boolean</b> data type. |
|[Add_String_Double](./add_string_double/) | Creates a new custom document property of the <b>PropertyType.Float</b> data type. |
|[AddLinkToContent](./addlinktocontent/) | Creates a new custom document property which links to content. |
|[UpdateLinkedPropertyValue](./updatelinkedpropertyvalue/) | Updates values of all custom properties that are linked to content(usecell value of linked range to update value of custom property). |
|[UpdateLinkedRange](./updatelinkedrange/) | Updates all ranges that are linked to custom properties(use the value ofcustom document property to update cell value of linked range). |
|[Get_Int](./get_int/) | Returns a DocumentProperty object by index. |
|[Contains](./contains/) | Returns true if a property with the specified name exists in the collection. |
|[IndexOf](./indexof/) | Gets the index of a property by name. |
|[Remove](./remove/) | Removes a property with the specified name from the collection. |
|[RemoveAt](./removeat/) | Removes a property at the specified index. |
|[Get_String](./get_string/) | Returns a DocumentProperty object by the name of the property. |
|[GetCount](./getcount/) |  |
