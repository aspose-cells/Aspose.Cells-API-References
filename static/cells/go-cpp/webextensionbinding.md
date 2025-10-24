##WebExtensionBinding Class
'WebExtensionBinding class. Encapsulates the object that represents webextensionbinding in Go.'
## WebExtensionBinding class
Represents a binding relationship between an Office Add-in and the data in the document.
```go
type WebExtensionBinding struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewWebExtensionBinding](./newwebextensionbinding/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetId](./getid/) | Gets and sets the binding identifier. |
|[SetId](./setid/) | Gets and sets the binding identifier. |
|[GetType](./gettype/) | Gets and sets the binding type. |
|[SetType](./settype/) | Gets and sets the binding type. |
|[GetAppref](./getappref/) | Gets and sets the binding key used to map the binding entry in this list with the bound data in the document. |
|[SetAppref](./setappref/) | Gets and sets the binding key used to map the binding entry in this list with the bound data in the document. |
