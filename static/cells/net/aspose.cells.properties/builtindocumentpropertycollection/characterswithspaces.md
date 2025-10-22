##BuiltInDocumentPropertyCollection.CharactersWithSpaces
BuiltInDocumentPropertyCollection property. Represents an estimate of the number of characters including spaces in the document
## BuiltInDocumentPropertyCollection.CharactersWithSpaces property
Represents an estimate of the number of characters (including spaces) in the document.
```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CharactersWithSpaces { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Properties;
using System;
public class BuiltInDocumentPropertyCollectionPropertyCharactersWithSpacesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access built-in document properties
BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
// Display current CharactersWithSpaces value
Console.WriteLine("Current CharactersWithSpaces value: " + properties.CharactersWithSpaces);
// Set a new value for CharactersWithSpaces
properties.CharactersWithSpaces = 1500;
Console.WriteLine("Updated CharactersWithSpaces value: " + properties.CharactersWithSpaces);
// Add some content to demonstrate property effect
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("This is a sample text to demonstrate document properties.");
worksheet.Cells["A2"].PutValue("The CharactersWithSpaces property represents estimated character count including spaces.");
// Save the workbook
workbook.Save("PropertyCharactersWithSpacesDemo.xlsx");
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
