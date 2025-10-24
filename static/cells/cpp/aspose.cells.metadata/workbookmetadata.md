##Aspose::Cells::Metadata::WorkbookMetadata class
'Aspose::Cells::Metadata::WorkbookMetadata class. Represents the meta data in C++.'
## WorkbookMetadata class
Represents the meta data.
```cpp
class WorkbookMetadata
```
## Methods
| Method | Description |
| --- | --- |
| [GetBuiltInDocumentProperties()](./getbuiltindocumentproperties/) | Returns a DocumentProperty collection that represents all the built-in document properties of the spreadsheet. |
| [GetCustomDocumentProperties()](./getcustomdocumentproperties/) | Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet. |
| [GetOptions()](./getoptions/) | Gets the options of the metadata. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const WorkbookMetadata\& src)](./operator_asm/) | operator= |
| [Save(const U16String\& fileName)](./save/) | Save the modified metadata to the file. |
| [Save(const char16_t* fileName)](./save/) | Save the modified metadata to the file. |
| [Save(const Vector \<uint8_t\>\& stream)](./save/) | Save the modified metadata to the stream. |
| [WorkbookMetadata(const U16String\& fileName, const MetadataOptions\& options)](./workbookmetadata/) | Create the meta data object. |
| [WorkbookMetadata(const char16_t* fileName, const MetadataOptions\& options)](./workbookmetadata/) | Create the meta data object. |
| [WorkbookMetadata(const Vector \<uint8_t\>\& stream, const MetadataOptions\& options)](./workbookmetadata/) | Create the meta data object. |
| [WorkbookMetadata(WorkbookMetadata_Impl* impl)](./workbookmetadata/) | Constructs from an implementation object. |
| [WorkbookMetadata(const WorkbookMetadata\& src)](./workbookmetadata/) | Copy constructor. |
| [~WorkbookMetadata()](./~workbookmetadata/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//The following example creates a WorkbookMetadata.
MetadataOptions options(MetadataType::Document_Properties);
WorkbookMetadata meta(u"book1.xlsx", options);
meta.GetCustomDocumentProperties().Add(u"test", u"test");
meta.Save(u"book2.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Metadata](../)
* Library [Aspose.Cells for C++](../../)
