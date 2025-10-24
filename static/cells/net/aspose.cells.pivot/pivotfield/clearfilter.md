##PivotField.ClearFilter
PivotField method. Clears filter setting on this pivot field
## PivotField.ClearFilter method
Clears filter setting on this pivot field.
```csharp
public void ClearFilter()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotFieldMethodClearFilterDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Category";
worksheet.Cells["A2"].Value = "Fruit";
worksheet.Cells["A3"].Value = "Vegetable";
worksheet.Cells["A4"].Value = "Fruit";
worksheet.Cells["A5"].Value = "Vegetable";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 100;
worksheet.Cells["B3"].Value = 200;
worksheet.Cells["B4"].Value = 150;
worksheet.Cells["B5"].Value = 300;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Get the pivot field
PivotField pivotField = pivotTable.RowFields[0];
try
{
// Apply a filter first to demonstrate clearing it
pivotField.FilterByLabel(PivotFilterType.CaptionEqual, "Fruit", null);
// Call ClearFilter method
pivotField.ClearFilter();
Console.WriteLine("ClearFilter method executed successfully");
Console.WriteLine("All filters have been removed from the pivot field");
// Refresh pivot table to show changes
pivotTable.RefreshData();
pivotTable.CalculateData();
}
catch (Exception ex)
{
Console.WriteLine($"Error executing ClearFilter method: {ex.Message}");
}
// Save the result
workbook.Save("PivotFieldMethodClearFilterDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
