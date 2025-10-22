##WebExtensionBindingCollection Class
'WebExtensionBindingCollection class. Encapsulates the object that represents webextensionbindingcollection in Go.'
## WebExtensionBindingCollection class
Represents the list of binding relationships between an Office Add-in and the data in the document.
```go
type WebExtensionBindingCollection struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewWebExtensionBindingCollection](./newwebextensionbindingcollection/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[Get](./get/) | Gets web extension binding relationship by the specific index. |
|[Add](./add/) | Adds an a binding relationship between an Office Add-in and the data in the document. |
|[GetCount](./getcount/) |  |
