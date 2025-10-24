##CustomDocumentPropertyCollection.AddLinkToContent
CustomDocumentPropertyCollection method. Creates a new custom document property which links to content
## CustomDocumentPropertyCollection.AddLinkToContent method
Creates a new custom document property which links to content.
```csharp
public DocumentProperty AddLinkToContent(string name, string source)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| source | String | The source of the property. It should be the name of named range. |
### Return Value
The newly created property object.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class CustomDocumentPropertyCollectionMethodAddLinkToContentWithStringStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set a value in cell A1 that will be linked
worksheet.Cells["A1"].PutValue("Linked Cell Value");
CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
// Add a regular property for comparison
customProperties.Add("RegularProperty", "Static Value");
// Add a linked property
customProperties.AddLinkToContent("LinkedProperty", "Sheet1!A1");
// Update the linked value
customProperties.UpdateLinkedRange();
// Display the properties
Console.WriteLine($"Regular Property: {customProperties["RegularProperty"].Value}");
Console.WriteLine($"Linked Property: {customProperties["LinkedProperty"].Value}");
workbook.Save("LinkedPropertyExample.xlsx");
}
}
}
```
### See Also
* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
