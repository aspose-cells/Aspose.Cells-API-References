##Workbook.CustomDocumentProperties
Workbook property. Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet
## Workbook.CustomDocumentProperties property
Returns a [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) collection that represents all the custom document properties of the spreadsheet.
```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class WorkbookPropertyCustomDocumentPropertiesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add custom document properties
workbook.CustomDocumentProperties.Add("Author", "John Doe");
workbook.CustomDocumentProperties.Add("Created Date", DateTime.Now);
workbook.CustomDocumentProperties.Add("Revision", 1);
workbook.CustomDocumentProperties.Add("Approved", true);
// Access and display the custom properties
Console.WriteLine("Custom Document Properties:");
foreach (Aspose.Cells.Properties.DocumentProperty prop in workbook.CustomDocumentProperties)
{
Console.WriteLine($"{prop.Name}: {prop.Value} ({prop.Type})");
}
// Save the workbook
workbook.Save("CustomDocumentPropertiesDemo.xlsx");
}
}
}
```
### See Also
* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
