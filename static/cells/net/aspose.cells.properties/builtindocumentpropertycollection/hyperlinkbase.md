##BuiltInDocumentPropertyCollection.HyperlinkBase
BuiltInDocumentPropertyCollection property. Gets or sets the hyperlinkbase property
## BuiltInDocumentPropertyCollection.HyperlinkBase property
Gets or sets the hyperlinkbase property.
```csharp
public string HyperlinkBase { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyHyperlinkBaseDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set the HyperlinkBase property
workbook.BuiltInDocumentProperties.HyperlinkBase = "http://www.example.com";
// Set some other property for demonstration
workbook.BuiltInDocumentProperties.Title = "Sample Workbook";
// Save the workbook
workbook.Save("HyperlinkBaseDemo.xlsx", SaveFormat.Xlsx);
// Load the saved workbook to verify properties
Workbook loadedWorkbook = new Workbook("HyperlinkBaseDemo.xlsx");
// Output the properties to console
Console.WriteLine("HyperlinkBase: " + loadedWorkbook.BuiltInDocumentProperties.HyperlinkBase);
Console.WriteLine("Title: " + loadedWorkbook.BuiltInDocumentProperties.Title);
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
