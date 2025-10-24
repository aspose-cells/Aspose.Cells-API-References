##PivotFilterCollection.ClearFilter
PivotFilterCollection method. Clear PivotFilter from the specific PivotField
## PivotFilterCollection.ClearFilter method
Clear PivotFilter from the specific PivotField
```csharp
public void ClearFilter(int fieldIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | the PivotField index |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotFilterCollectionMethodClearFilterWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B1"].Value = "Quantity";
worksheet.Cells["B2"].Value = 10;
worksheet.Cells["B3"].Value = 5;
worksheet.Cells["B4"].Value = 8;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Add filter to pivot table
PivotFilterCollection filters = pivotTable.PivotFilters;
filters.AddLabelFilter(0, PivotFilterType.Count, "Apple", null);
try
{
// Call ClearFilter method with field index parameter
filters.ClearFilter(0);
Console.WriteLine("Pivot filter cleared successfully for field index 0");
// Verify filter was cleared
Console.WriteLine($"Number of filters after clearing: {filters.Count}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing ClearFilter method: {ex.Message}");
}
// Save the workbook
workbook.Save("PivotFilterCollectionMethodClearFilterWithInt32Demo.xlsx");
}
}
}
```
### See Also
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
