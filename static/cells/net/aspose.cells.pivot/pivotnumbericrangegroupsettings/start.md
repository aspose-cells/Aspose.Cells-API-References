##PivotNumbericRangeGroupSettings.Start
PivotNumbericRangeGroupSettings property. Gets the start number of the group
## PivotNumbericRangeGroupSettings.Start property
Gets the start number of the group.
```csharp
public double Start { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotNumbericRangeGroupSettingsPropertyStartDemo
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
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:A6", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
// Group the numeric field
PivotField pivotField = pivotTable.RowFields[0];
pivotField.GroupBy(10, 50, 10, true);
// Get the numeric range group settings
PivotNumbericRangeGroupSettings groupSettings = pivotField.GroupSettings as PivotNumbericRangeGroupSettings;
// Display the current Start value
Console.WriteLine("Current Start value: " + groupSettings.Start);
// Note: Start is read-only, so we can't set it directly
// To change the grouping, we need to recreate the grouping with new parameters
pivotField.Ungroup();
pivotField.GroupBy(15, 55, 10, true); // New start value of 15
// Get the updated group settings
groupSettings = pivotField.GroupSettings as PivotNumbericRangeGroupSettings;
Console.WriteLine("Updated Start value: " + groupSettings.Start);
// Save the workbook
workbook.Save("PivotNumbericRangeGroupSettingsPropertyStartDemo.xlsx");
}
}
}
```
### See Also
* class [PivotNumbericRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
