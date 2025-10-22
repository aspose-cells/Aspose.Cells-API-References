##PivotNumbericRangeGroupSettings.End
PivotNumbericRangeGroupSettings property. Gets the end number of the group
## PivotNumbericRangeGroupSettings.End property
Gets the end number of the group.
```csharp
public double End { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotNumbericRangeGroupSettingsPropertyEndDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Amount");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["A3"].PutValue(20);
worksheet.Cells["A4"].PutValue(30);
worksheet.Cells["A5"].PutValue(40);
worksheet.Cells["A6"].PutValue(50);
worksheet.Cells["A7"].PutValue(60);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:A7", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
// Group numeric field
PivotField pivotField = pivotTable.RowFields[0];
pivotField.GroupBy(10, 60, 10, false);
// Get numeric range group settings
PivotNumbericRangeGroupSettings groupSettings = pivotField.GroupSettings as PivotNumbericRangeGroupSettings;
// Display the current End value
Console.WriteLine("Current End value: " + groupSettings.End);
// Note: End property is read-only, so we cannot set it directly
// To change the end value, we need to recreate the grouping with new parameters
pivotField.Ungroup();
pivotField.GroupBy(10, 50, 10, false); // New end value is 50
// Get updated group settings
groupSettings = pivotField.GroupSettings as PivotNumbericRangeGroupSettings;
Console.WriteLine("Updated End value: " + groupSettings.End);
// Save the result
workbook.Save("PivotNumbericRangeGroupSettingsPropertyEndDemo.xlsx");
}
}
}
```
### See Also
* class [PivotNumbericRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
