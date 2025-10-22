##BuiltInDocumentPropertyCollection.Characters
BuiltInDocumentPropertyCollection property. Represents an estimate of the number of characters in the document
## BuiltInDocumentPropertyCollection.Characters property
Represents an estimate of the number of characters in the document.
```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Characters { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Properties;
using System;
public class BuiltInDocumentPropertyCollectionPropertyCharactersDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access built-in document properties
BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
// Display current Characters value (obsolete property)
Console.WriteLine("Current Characters value: " + properties.Characters);
// Set a new value for Characters (obsolete property)
properties.Characters = 1500;
Console.WriteLine("Updated Characters value: " + properties.Characters);
// Add some content to demonstrate property effect
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("This is a sample text to demonstrate document properties.");
// Save the workbook
workbook.Save("PropertyCharactersDemo.xlsx");
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
