##WorkbookMetadata Class
'WorkbookMetadata class. Encapsulates the object that represents workbookmetadata in Go.'
## WorkbookMetadata class
Represents the meta data.
```go
type WorkbookMetadata struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewWorkbookMetadata_String_MetadataOptions](./newworkbookmetadata_string_metadataoptions/) | Create the meta data object. |
|[NewWorkbookMetadata_Stream_MetadataOptions](./newworkbookmetadata_stream_metadataoptions/) | Create the meta data object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetOptions](./getoptions/) | Gets the options of the metadata. |
|[GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | Returns a DocumentProperty collection that represents all the  built-in document properties of the spreadsheet. |
|[GetCustomDocumentProperties](./getcustomdocumentproperties/) | Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet. |
|[Save_String](./save_string/) | Save the modified metadata to the file. |
|[Save_Stream](./save_stream/) | Save the modified metadata to the stream. |
