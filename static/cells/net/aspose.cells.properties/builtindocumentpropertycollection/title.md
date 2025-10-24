##BuiltInDocumentPropertyCollection.Title
BuiltInDocumentPropertyCollection property. Gets or sets the title of the document
## BuiltInDocumentPropertyCollection.Title property
Gets or sets the title of the document.
```csharp
public string Title { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyTitleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set the Title property
workbook.BuiltInDocumentProperties.Title = "Sample Document Title";
// Display the Title property
Console.WriteLine("Document Title: " + workbook.BuiltInDocumentProperties.Title);
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
