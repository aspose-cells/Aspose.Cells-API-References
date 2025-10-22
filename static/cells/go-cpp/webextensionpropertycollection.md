##WebExtensionPropertyCollection Class
'WebExtensionPropertyCollection class. Encapsulates the object that represents webextensionpropertycollection in Go.'
## WebExtensionPropertyCollection class
Represents the list of web extension properties.
```go
type WebExtensionPropertyCollection struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewWebExtensionPropertyCollection](./newwebextensionpropertycollection/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[Get_Int](./get_int/) | Gets the property of web extension by the index. |
|[Get_String](./get_string/) | Gets the property of web extension. |
|[Add](./add/) | Adds web extension property. |
|[RemoveAt](./removeat/) | Remove the property by the name. |
|[GetCount](./getcount/) |  |
