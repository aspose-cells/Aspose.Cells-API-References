##BuiltInDocumentPropertyCollection.Paragraphs
BuiltInDocumentPropertyCollection property. Represents an estimate of the number of paragraphs in the document
## BuiltInDocumentPropertyCollection.Paragraphs property
Represents an estimate of the number of paragraphs in the document.
```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Paragraphs { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Properties;
using System;
public class BuiltInDocumentPropertyCollectionPropertyParagraphsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access built-in document properties
BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
// Display current Paragraphs value (obsolete property)
Console.WriteLine("Current Paragraphs value: " + properties.Paragraphs);
// Set a new value for Paragraphs (obsolete property)
properties.Paragraphs = 15;
Console.WriteLine("Updated Paragraphs value: " + properties.Paragraphs);
// Add some content to demonstrate property effect
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("This is paragraph 1");
worksheet.Cells["A2"].PutValue("This is paragraph 2");
worksheet.Cells["A3"].PutValue("This is paragraph 3");
// Save the workbook
workbook.Save("PropertyParagraphsDemo.xlsx");
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
