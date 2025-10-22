##WorkbookMetadata class
## WorkbookMetadata class
Represents the meta data.
The WorkbookMetadata type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self, file_name, options)`](/cells/python-net/aspose.cells.metadata/workbookmetadata/__init__/#system.string-aspose.cells.metadata.metadataoptions) | Create the meta data object. |
| [`__init__(self, stream, options)`](/cells/python-net/aspose.cells.metadata/workbookmetadata/__init__/#io.rawiobase-aspose.cells.metadata.metadataoptions) | Create the meta data object. |
### Properties
| Property | Description |
| :- | :- |
| [options](/cells/python-net/aspose.cells.metadata/workbookmetadata/options) | Gets the options of the metadata. |
| [built_in_document_properties](/cells/python-net/aspose.cells.metadata/workbookmetadata/built_in_document_properties) | Returns a [`DocumentProperty`](/cells/python-net/aspose.cells.properties/documentproperty) collection that represents all the  built-in document properties of the spreadsheet. |
| [custom_document_properties](/cells/python-net/aspose.cells.metadata/workbookmetadata/custom_document_properties) | Returns a [`DocumentProperty`](/cells/python-net/aspose.cells.properties/documentproperty) collection that represents all the custom document properties of the spreadsheet. |
### Methods
| Method | Description |
| :- | :- |
| [`save(self, file_name)`](/cells/python-net/aspose.cells.metadata/workbookmetadata/save/#system.string) | Save the modified metadata to the file. |
| [`save(self, stream)`](/cells/python-net/aspose.cells.metadata/workbookmetadata/save/#io.rawiobase) | Save the modified metadata to the stream. |
### Example
The following example creates a WorkbookMetadata.
```python
from aspose.cells.metadata import MetadataOptions, MetadataType, WorkbookMetadata
options = MetadataOptions(MetadataType.DOCUMENT_PROPERTIES)
meta = WorkbookMetadata("book1.xlsx", options)
meta.custom_document_properties.add("test", "test")
meta.save("book2.xlsx")
```
### See Also
* module [`aspose.cells.metadata`](..)
* class [`DocumentProperty`](/cells/python-net/aspose.cells.properties/documentproperty)
