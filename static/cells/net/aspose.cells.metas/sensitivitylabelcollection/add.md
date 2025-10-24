##SensitivityLabelCollection.Add
SensitivityLabelCollection method. Adds a sensitivity label
## SensitivityLabelCollection.Add method
Adds a sensitivity label.
```csharp
public int Add(string id, bool isEnabled, SensitivityLabelAssignmentType methodType, string siteId,
SensitivityLabelMarkType markType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| id | String | The id of the label. |
| isEnabled | Boolean | Indicates whether this sensitivity label is enabled. |
| methodType | SensitivityLabelAssignmentType | The assignment method type. |
| siteId | String | The id of the site. |
| markType | SensitivityLabelMarkType | The mark type. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Metas;
using System;
public class SensitivityLabelCollectionMethodAddWithStringBooleanSensitivityLabelADemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a new SensitivityLabelCollection
var sensitivityLabels = new SensitivityLabelCollection();
try
{
// Call the Add method with specific parameters
int index = sensitivityLabels.Add(
id: "Confidential",
isEnabled: true,
methodType: SensitivityLabelAssignmentType.Privileged,
siteId: "Contoso",
markType: SensitivityLabelMarkType.Watermark);
Console.WriteLine($"Sensitivity label added at index: {index}");
// Add some data to demonstrate the effect
worksheet.Cells["A1"].Value = "Confidential Data";
worksheet.Cells["A2"].Value = "This document contains sensitive information";
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Add method: {ex.Message}");
}
// Save the result
workbook.Save("SensitivityLabelAddDemo.xlsx");
}
}
}
```
### See Also
* enum [SensitivityLabelAssignmentType](../../sensitivitylabelassignmenttype/)
* enum [SensitivityLabelMarkType](../../sensitivitylabelmarktype/)
* class [SensitivityLabelCollection](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)
