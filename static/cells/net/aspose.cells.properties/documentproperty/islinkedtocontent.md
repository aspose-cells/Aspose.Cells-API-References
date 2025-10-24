##DocumentProperty.IsLinkedToContent
DocumentProperty property. Indicates whether this property is linked to content
## DocumentProperty.IsLinkedToContent property
Indicates whether this property is linked to content
```csharp
public bool IsLinkedToContent { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class DocumentPropertyPropertyIsLinkedToContentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add sample data to cells
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].Value = "Company Name";
worksheet.Cells["B1"].Value = "Company Address";
// Create linked custom document properties
workbook.CustomDocumentProperties.AddLinkToContent("Company", "A1");
workbook.CustomDocumentProperties.AddLinkToContent("Address", "B1");
// Get and check the IsLinkedToContent property
DocumentProperty companyProp = workbook.CustomDocumentProperties["Company"];
Console.WriteLine($"Is 'Company' property linked to content: {companyProp.IsLinkedToContent}");
Console.WriteLine($"Linked source: {companyProp.Source}");
Console.WriteLine($"Current value: {companyProp.Value}");
// Update cell value and refresh linked properties
worksheet.Cells["A1"].Value = "Updated Company Name";
workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();
// Verify the property was updated
Console.WriteLine($"Updated value: {companyProp.Value}");
// Save the workbook
workbook.Save("LinkedPropertiesDemo.xlsx");
}
}
}
```
### See Also
* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
