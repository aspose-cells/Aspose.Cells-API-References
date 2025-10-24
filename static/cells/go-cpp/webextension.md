##WebExtension Class
'WebExtension class. Encapsulates the object that represents webextension in Go.'
## WebExtension class
Represents an Office Add-in instance.
```go
type WebExtension struct  {
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
|[GetId](./getid/) | Gets and sets the uniquely identifies the Office Add-in instance in the current document. |
|[SetId](./setid/) | Gets and sets the uniquely identifies the Office Add-in instance in the current document. |
|[IsFrozen](./isfrozen/) | Indicates whether the user can interact with the Office Add-in or not. |
|[SetIsFrozen](./setisfrozen/) | Indicates whether the user can interact with the Office Add-in or not. |
|[GetReference](./getreference/) | Get the primary reference to an Office Add-in. |
|[GetAlterReferences](./getalterreferences/) | Gets a list of alter references. |
|[GetProperties](./getproperties/) | Gets all properties of web extension. |
|[GetBindings](./getbindings/) | Gets all bindings relationship between an Office Add-in and the data in the document. |
