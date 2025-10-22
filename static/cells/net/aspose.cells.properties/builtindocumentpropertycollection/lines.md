##BuiltInDocumentPropertyCollection.Lines
BuiltInDocumentPropertyCollection property. Represents an estimate of the number of lines in the document
## BuiltInDocumentPropertyCollection.Lines property
Represents an estimate of the number of lines in the document.
```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Lines { get; set; }
```
### Remarks
Aspose.Cells does not update this property when you modify the document.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Properties;
using System;
public class BuiltInDocumentPropertyCollectionPropertyLinesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access built-in document properties
BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
// Display current Lines value (estimate of number of lines in document)
Console.WriteLine("Current Lines value: " + properties.Lines);
// Set a new value for Lines property
properties.Lines = 150;
// Add some content to demonstrate the property's purpose
Worksheet worksheet = workbook.Worksheets[0];
for (int i = 0; i < 50; i++)
{
worksheet.Cells[i, 0].Value = "Line " + (i + 1);
}
// Save the workbook
workbook.Save("PropertyLinesDemo.xlsx");
// Note: The Lines property is an estimate and won't automatically update with actual content
// It's primarily used for document metadata purposes
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
