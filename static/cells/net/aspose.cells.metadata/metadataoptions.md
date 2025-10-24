##Class MetadataOptions
Aspose.Cells.Metadata.MetadataOptions class. Represents the options of loading metadata of the file
## MetadataOptions class
Represents the options of loading metadata of the file.
```csharp
public class MetadataOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [MetadataOptions](metadataoptions/)(MetadataType) | Creates an options of loading the metadata. |
## Properties
| Name | Description |
| --- | --- |
| [KeyLength](../../aspose.cells.metadata/metadataoptions/keylength/) { get; set; } | The key length. |
| [MetadataType](../../aspose.cells.metadata/metadataoptions/metadatatype/) { get; } | Gets and sets the type of the metadata which is loading. |
| [Password](../../aspose.cells.metadata/metadataoptions/password/) { get; set; } | Represents Workbook file encryption password. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Metadata;
using System;
public class MetadataOptionsDemo
{
public static void MetadataOptionsExample()
{
// Create an instance of MetadataOptions with a specific MetadataType
MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
// Set properties
options.Password = "your_password";
options.KeyLength = 256;
// Load metadata from an existing workbook
WorkbookMetadata metadata = new WorkbookMetadata("MetadataOptionsExample_original.xlsx", options);
// Add a custom document property
metadata.CustomDocumentProperties.Add("Author", "John Doe");
// Save the metadata changes to a new file
metadata.Save("MetadataOptionsExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)
