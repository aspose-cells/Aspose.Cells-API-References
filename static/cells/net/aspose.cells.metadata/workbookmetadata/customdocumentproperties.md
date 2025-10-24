##WorkbookMetadata.CustomDocumentProperties
WorkbookMetadata property. Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet
## WorkbookMetadata.CustomDocumentProperties property
Returns a [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) collection that represents all the custom document properties of the spreadsheet.
```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;
namespace AsposeCellsExamples
{
public class WorkbookMetadataPropertyCustomDocumentPropertiesDemo
{
public static void Run()
{
// Source and destination paths
string sourcePath = "example.xlsx";
string destPath = "output.xlsx";
// Create metadata options for document properties
MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
// Initialize workbook metadata
WorkbookMetadata meta = new WorkbookMetadata(sourcePath, options);
// Add custom document property
meta.CustomDocumentProperties.Add("Author", "John Doe");
// Save the workbook with metadata
meta.Save(destPath);
// Verify the custom property
Workbook workbook = new Workbook(destPath);
Console.WriteLine("Custom Property Value: " +
workbook.CustomDocumentProperties["Author"].Value);
}
}
}
```
### See Also
* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)
