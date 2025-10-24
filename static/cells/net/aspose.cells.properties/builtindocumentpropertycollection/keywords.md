##BuiltInDocumentPropertyCollection.Keywords
BuiltInDocumentPropertyCollection property. Gets or sets the document keywords
## BuiltInDocumentPropertyCollection.Keywords property
Gets or sets the document keywords.
```csharp
public string Keywords { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyKeywordsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set the Keywords property
workbook.BuiltInDocumentProperties.Keywords = "Sample Keywords, Aspose.Cells, Demo";
// Save the workbook
workbook.Save("output_keywords.xlsx");
// Load the saved workbook to verify the Keywords property
Workbook loadedWorkbook = new Workbook("output_keywords.xlsx");
// Display the Keywords property
Console.WriteLine("Document Keywords: " + loadedWorkbook.BuiltInDocumentProperties.Keywords);
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
