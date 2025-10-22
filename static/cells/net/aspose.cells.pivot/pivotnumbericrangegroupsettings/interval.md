##PivotNumbericRangeGroupSettings.Interval
PivotNumbericRangeGroupSettings property. Gets the interval of the group
## PivotNumbericRangeGroupSettings.Interval property
Gets the interval of the group.
```csharp
public double Interval { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotNumbericRangeGroupSettingsPropertyIntervalDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue(15);
worksheet.Cells["A3"].PutValue(25);
worksheet.Cells["A4"].PutValue(35);
worksheet.Cells["A5"].PutValue(45);
worksheet.Cells["A6"].PutValue(55);
worksheet.Cells["A7"].PutValue(65);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:A7", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
// Group numeric field with initial interval of 15
PivotField pivotField = pivotTable.RowFields[0];
pivotField.GroupBy(15, 75, 15, false);
// Get numeric range group settings
PivotNumbericRangeGroupSettings groupSettings = pivotField.GroupSettings as PivotNumbericRangeGroupSettings;
// Display current interval value
Console.WriteLine("Initial grouping interval: " + groupSettings.Interval);
// Note: Interval is read-only, so we need to recreate grouping to change it
pivotField.Ungroup();
pivotField.GroupBy(15, 75, 20, false); // New interval of 20
// Get updated group settings
groupSettings = pivotField.GroupSettings as PivotNumbericRangeGroupSettings;
Console.WriteLine("Updated grouping interval: " + groupSettings.Interval);
// Save the result
workbook.Save("PivotNumbericRangeGroupSettingsPropertyIntervalDemo.xlsx");
}
}
}
```
### See Also
* class [PivotNumbericRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
