##MetadataOptions.Password
MetadataOptions property. Represents Workbook file encryption password
## MetadataOptions.Password property
Represents Workbook file encryption password.
```csharp
public string Password { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;
namespace AsposeCellsExamples
{
public class MetadataOptionsPropertyPasswordDemo
{
public static void Run()
{
// Create metadata options with password protection
MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
options.Password = "secure_password123";
// Create a new workbook and save it first
Workbook workbook = new Workbook();
string filePath = "ProtectedMetadata.xlsx";
workbook.Save(filePath);
// Load metadata from the saved file
WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);
// Add custom document property
metadata.CustomDocumentProperties.Add("CreatedBy", "MetadataDemo");
// Save with metadata
metadata.Save(filePath);
}
}
}
```
### See Also
* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)
