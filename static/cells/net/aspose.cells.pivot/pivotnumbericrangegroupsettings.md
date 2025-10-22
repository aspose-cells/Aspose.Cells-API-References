##Class PivotNumbericRangeGroupSettings
Aspose.Cells.Pivot.PivotNumbericRangeGroupSettings class. Represents the numberic range group of the pivot field
## PivotNumbericRangeGroupSettings class
Represents the numberic range group of the pivot field.
```csharp
public class PivotNumbericRangeGroupSettings : PivotFieldGroupSettings
```
## Properties
| Name | Description |
| --- | --- |
| [End](../../aspose.cells.pivot/pivotnumbericrangegroupsettings/end/) { get; } | Gets the end number of the group. |
| [Interval](../../aspose.cells.pivot/pivotnumbericrangegroupsettings/interval/) { get; } | Gets the interval of the group. |
| [Start](../../aspose.cells.pivot/pivotnumbericrangegroupsettings/start/) { get; } | Gets the start number of the group. |
| override [Type](../../aspose.cells.pivot/pivotnumbericrangegroupsettings/type/) { get; } | Gets the group type. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotClassPivotNumbericRangeGroupSettingsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Amount";
worksheet.Cells["A2"].Value = 10;
worksheet.Cells["A3"].Value = 20;
worksheet.Cells["A4"].Value = 30;
worksheet.Cells["A5"].Value = 40;
worksheet.Cells["A6"].Value = 50;
worksheet.Cells["A7"].Value = 60;
worksheet.Cells["A8"].Value = 70;
worksheet.Cells["A9"].Value = 80;
worksheet.Cells["A10"].Value = 90;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:A10", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
// Group numeric range in pivot field
PivotField pivotField = pivotTable.RowFields[0];
pivotField.GroupBy(0, 100, 20, false);
// Get the group settings
PivotNumbericRangeGroupSettings groupSettings = pivotField.GroupSettings as PivotNumbericRangeGroupSettings;
// Display group settings information
Console.WriteLine("Group Type: " + groupSettings.Type);
Console.WriteLine("Start Value: " + groupSettings.Start);
Console.WriteLine("End Value: " + groupSettings.End);
Console.WriteLine("Interval: " + groupSettings.Interval);
// Save the workbook
workbook.Save("PivotNumbericRangeGroupSettingsDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFieldGroupSettings](../pivotfieldgroupsettings/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
