##PivotNumbericRangeGroupSettings.Type
PivotNumbericRangeGroupSettings property. Gets the group type
## PivotNumbericRangeGroupSettings.Type property
Gets the group type.
```csharp
public override PivotFieldGroupType Type { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotNumbericRangeGroupSettingsPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].Value = "Amount";
worksheet.Cells["A2"].Value = 10;
worksheet.Cells["A3"].Value = 20;
worksheet.Cells["A4"].Value = 30;
worksheet.Cells["A5"].Value = 40;
worksheet.Cells["A6"].Value = 50;
// Create a pivot table
int index = worksheet.PivotTables.Add("A1:A6", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
// Group the data by numeric range
PivotField pivotField = pivotTable.RowFields[0];
pivotField.GroupBy(10, 50, 10, false);
// Get the numeric range group settings
PivotNumbericRangeGroupSettings groupSettings = (PivotNumbericRangeGroupSettings)pivotField.GroupSettings;
// Display the current Type value
Console.WriteLine("Current Type value: " + groupSettings.Type);
// Demonstrate how the Type affects the grouping
if (groupSettings.Type == PivotFieldGroupType.NumbericRange)
{
Console.WriteLine("The field is grouped by numeric range:");
Console.WriteLine("Start: " + groupSettings.Start);
Console.WriteLine("End: " + groupSettings.End);
Console.WriteLine("Interval: " + groupSettings.Interval);
}
// Save the workbook
workbook.Save("PivotNumbericRangeGroupSettingsPropertyTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotFieldGroupType](../../pivotfieldgrouptype/)
* class [PivotNumbericRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
