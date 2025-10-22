##MetadataOptions Class
'MetadataOptions class. Encapsulates the object that represents metadataoptions in Go.'
## MetadataOptions class
Represents the options of loading metadata of the file.
```go
type MetadataOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewMetadataOptions](./newmetadataoptions/) | Creates an options of loading the metadata. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetMetadataType](./getmetadatatype/) | Gets and sets the type of the metadata which is loading. |
|[GetPassword](./getpassword/) | Represents Workbook file encryption password. |
|[SetPassword](./setpassword/) | Represents Workbook file encryption password. |
|[GetKeyLength](./getkeylength/) | The key length. |
|[SetKeyLength](./setkeylength/) | The key length. |
