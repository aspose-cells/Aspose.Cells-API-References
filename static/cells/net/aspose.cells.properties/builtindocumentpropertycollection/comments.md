##BuiltInDocumentPropertyCollection.Comments
BuiltInDocumentPropertyCollection property. Gets or sets the document comments
## BuiltInDocumentPropertyCollection.Comments property
Gets or sets the document comments.
```csharp
public string Comments { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyCommentsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access built-in document properties
BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
// Set the Comments property
properties.Comments = "This is a sample comment for demonstration.";
// Display the Comments property
Console.WriteLine("Document Comments: " + properties.Comments);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
