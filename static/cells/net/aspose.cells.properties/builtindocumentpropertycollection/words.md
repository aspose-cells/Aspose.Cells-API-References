##BuiltInDocumentPropertyCollection.Words
BuiltInDocumentPropertyCollection property. Represents an estimate of the number of words in the document
## BuiltInDocumentPropertyCollection.Words property
Represents an estimate of the number of words in the document.
```csharp
public int Words { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyWordsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the built-in document properties
BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;
// Set the Words property
builtInProperties.Words = 250;
// Add some content to the worksheet
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("This is a sample document");
worksheet.Cells["A2"].PutValue("Demonstrating the Words property");
worksheet.Cells["A3"].PutValue("Total words will be set to 250");
// Save the workbook
workbook.Save("DocumentWithWordsProperty.xlsx");
Console.WriteLine("Document created with Words property set to: " + builtInProperties.Words);
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
