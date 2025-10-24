##WebExtensionReference Class
'WebExtensionReference class. Encapsulates the object that represents webextensionreference in Go.'
## WebExtensionReference class
Represents identify the provider location and version of the extension.
```go
type WebExtensionReference struct  {
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
|[GetId](./getid/) | Gets and sets the identifier associated with the Office Add-in within a catalog provider.The identifier MUST be unique within a catalog provider. |
|[SetId](./setid/) | Gets and sets the identifier associated with the Office Add-in within a catalog provider.The identifier MUST be unique within a catalog provider. |
|[GetVersion](./getversion/) | Gets and sets the version. |
|[SetVersion](./setversion/) | Gets and sets the version. |
|[GetStoreName](./getstorename/) | Gets and sets the instance of the marketplace where the Office Add-in is stored. . |
|[SetStoreName](./setstorename/) | Gets and sets the instance of the marketplace where the Office Add-in is stored. . |
|[GetStoreType](./getstoretype/) | Gets and sets the type of marketplace that the store attribute identifies. |
|[SetStoreType](./setstoretype/) | Gets and sets the type of marketplace that the store attribute identifies. |
