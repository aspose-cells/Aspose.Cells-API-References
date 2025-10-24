##BuiltInDocumentPropertyCollection.ContentStatus
BuiltInDocumentPropertyCollection property. Gets or sets the content status of the document
## BuiltInDocumentPropertyCollection.ContentStatus property
Gets or sets the content status of the document.
```csharp
public string ContentStatus { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyContentStatusDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set built-in document properties including ContentStatus
workbook.BuiltInDocumentProperties.ContentStatus = "Draft";
workbook.BuiltInDocumentProperties.Author = "John Doe";
workbook.BuiltInDocumentProperties.Title = "Sample Document";
// Save the workbook
workbook.Save("DocumentWithContentStatus.xlsx", SaveFormat.Xlsx);
// Load the saved workbook to verify properties
Workbook loadedWorkbook = new Workbook("DocumentWithContentStatus.xlsx");
// Display the ContentStatus property
Console.WriteLine("Content Status: " + loadedWorkbook.BuiltInDocumentProperties.ContentStatus);
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
