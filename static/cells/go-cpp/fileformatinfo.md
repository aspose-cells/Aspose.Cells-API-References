##FileFormatInfo Class
'FileFormatInfo class. Encapsulates the object that represents fileformatinfo in Go.'
## FileFormatInfo class
Contains data returned by <see cref="FileFormatUtil"/> file format detection methods.
```go
type FileFormatInfo struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewFileFormatInfo](./newfileformatinfo/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[IsProtectedByRMS](./isprotectedbyrms/) | Gets whether the file is protected by Microsoft Rights Management Server. |
|[IsEncrypted](./isencrypted/) | Returns true if the document is encrypted and requires a password to open. |
|[GetFileFormatType](./getfileformattype/) | Gets the detected file format. |
|[GetLoadFormat](./getloadformat/) | Gets the detected load format. |
