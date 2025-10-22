##BuiltInDocumentPropertyCollection.ContentType
BuiltInDocumentPropertyCollection property. Gets or sets the content type of the document
## BuiltInDocumentPropertyCollection.ContentType property
Gets or sets the content type of the document.
```csharp
public string ContentType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyContentTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set the ContentType property
workbook.BuiltInDocumentProperties.ContentType = "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet";
// Display the ContentType property
Console.WriteLine("ContentType: " + workbook.BuiltInDocumentProperties.ContentType);
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
