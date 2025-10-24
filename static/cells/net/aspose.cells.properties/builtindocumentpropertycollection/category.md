##BuiltInDocumentPropertyCollection.Category
BuiltInDocumentPropertyCollection property. Gets or sets the category of the document
## BuiltInDocumentPropertyCollection.Category property
Gets or sets the category of the document.
```csharp
public string Category { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyCategoryDemo
{
public static void Run()
{
// Create a new workbook
var workbook = new Workbook();
// Set built-in document properties
workbook.BuiltInDocumentProperties.Category = "Financial Report";
workbook.BuiltInDocumentProperties.ContentStatus = "Final";
// Save to memory stream
var stream = new MemoryStream();
workbook.Save(stream, SaveFormat.Xlsx);
// Load the workbook back from stream
stream.Position = 0;
var loadedWorkbook = new Workbook(stream);
// Display the properties
Console.WriteLine("Category: " + loadedWorkbook.BuiltInDocumentProperties.Category);
Console.WriteLine("Content Status: " + loadedWorkbook.BuiltInDocumentProperties.ContentStatus);
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
