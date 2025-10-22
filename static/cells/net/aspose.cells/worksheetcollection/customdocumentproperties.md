##WorksheetCollection.CustomDocumentProperties
WorksheetCollection property. Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet
## WorksheetCollection.CustomDocumentProperties property
Returns a [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) collection that represents all the custom document properties of the spreadsheet.
```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionPropertyCustomDocumentPropertiesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add custom document properties
workbook.Worksheets.CustomDocumentProperties.Add("Author", "John Doe");
workbook.Worksheets.CustomDocumentProperties.Add("CreatedDate", DateTime.Now);
workbook.Worksheets.CustomDocumentProperties.Add("Version", 1.2);
// Access and display the properties
Console.WriteLine("Author: " + workbook.Worksheets.CustomDocumentProperties["Author"]);
Console.WriteLine("Created: " + workbook.Worksheets.CustomDocumentProperties["CreatedDate"]);
Console.WriteLine("Version: " + workbook.Worksheets.CustomDocumentProperties["Version"]);
}
}
}
```
### See Also
* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
