##PivotTable.SetUngroup
PivotTable method. Sets ungroup by the PivotTable
## SetUngroup(int) {#setungroup_1}
Sets ungroup by the PivotTable
```csharp
[Obsolete("Use PivotField.Ungroup() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetUngroup(int baseFieldIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | Int32 | The row or column field index in the base fields |
### Remarks
NOTE: This method is now obsolete. Instead, please use PivotField.Ungroup() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTableMethodSetUngroupWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].PutValue("Date");
worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
worksheet.Cells["A3"].PutValue(new DateTime(2023, 1, 2));
worksheet.Cells["A4"].PutValue(new DateTime(2023, 1, 3));
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["B3"].PutValue(1500);
worksheet.Cells["B4"].PutValue(2000);
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to the pivot table
int dateFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Group the date field by days (this will create a grouped field)
pivotTable.RowFields[0].GroupBy(
new DateTime(2023, 1, 1),
new DateTime(2023, 1, 3),
new[] { PivotGroupByType.Days },
1,
false);
try
{
// Call SetUngroup method with the base field index
pivotTable.SetUngroup(dateFieldIndex);
Console.WriteLine("Date field ungrouped successfully");
// Calculate data to update the pivot table
pivotTable.CalculateData();
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetUngroup method: {ex.Message}");
}
// Save the result
workbook.Save("PivotTableSetUngroupDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## SetUngroup(PivotField) {#setungroup}
Sets ungroup by the PivotTable
```csharp
[Obsolete("Use PivotField.Ungroup() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetUngroup(PivotField pivotField)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | PivotField | The row or column field in the base fields |
### Remarks
NOTE: This method is now obsolete. Instead, please use PivotField.Ungroup() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTableMethodSetUngroupWithPivotFieldDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["A5"].Value = "Apple";
worksheet.Cells["B1"].Value = "Quantity";
worksheet.Cells["B2"].Value = 10;
worksheet.Cells["B3"].Value = 15;
worksheet.Cells["B4"].Value = 20;
worksheet.Cells["B5"].Value = 5;
// Create a pivot table
int index = worksheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Group the row field (Fruit) by first letter
PivotField rowField = pivotTable.RowFields[0];
pivotTable.SetAutoGroupField(rowField);
try
{
// Call SetUngroup to ungroup the previously grouped field
pivotTable.SetUngroup(rowField);
Console.WriteLine("SetUngroup method executed successfully on the PivotField");
// Show the effect - the grouping should be removed
Console.WriteLine("PivotTable row field is now ungrouped");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetUngroup method: {ex.Message}");
}
// Save the result
workbook.Save("PivotTableSetUngroupDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
