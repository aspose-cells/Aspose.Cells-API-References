##DocumentProperty.Value
DocumentProperty property. Gets or sets the value of the property
## DocumentProperty.Value property
Gets or sets the value of the property.
```csharp
public object Value { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DocumentPropertyPropertyValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access built-in document properties
var hyperlinkBase = workbook.Worksheets.BuiltInDocumentProperties["HyperlinkBase"];
hyperlinkBase.Value = "http://www.example.com";
var title = workbook.Worksheets.BuiltInDocumentProperties["Title"];
title.Value = "Sample Document Title";
// Save the workbook
workbook.Save("DocumentPropertiesDemo.xlsx");
// Display the set values
Console.WriteLine("HyperlinkBase: " + hyperlinkBase.Value);
Console.WriteLine("Title: " + title.Value);
}
}
}
```
### See Also
* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
