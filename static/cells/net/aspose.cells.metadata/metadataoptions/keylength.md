##MetadataOptions.KeyLength
MetadataOptions property. The key length
## MetadataOptions.KeyLength property
The key length.
```csharp
public int KeyLength { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;
namespace AsposeCellsExamples
{
public class MetadataOptionsPropertyKeyLengthDemo
{
public static void Run()
{
// Create metadata options with document properties type
MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
// Set encryption properties including KeyLength
options.Password = "secure_password";
options.KeyLength = 256; // Using 256-bit encryption
// Create metadata for a new workbook
WorkbookMetadata metadata = new WorkbookMetadata("sample.xlsx", options);
// Add custom property
metadata.CustomDocumentProperties.Add("CreatedBy", "MetadataDemo");
// Save with encryption
metadata.Save("encrypted_sample.xlsx");
}
}
}
```
### See Also
* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)
