##PivotField.FilterByValue
PivotField method. Filters by values of data pivot field
## PivotField.FilterByValue method
Filters by values of data pivot field.
```csharp
public PivotFilter FilterByValue(int valueFieldIndex, PivotFilterType type, double value1,
double value2)
```
| Parameter | Type | Description |
| --- | --- | --- |
| valueFieldIndex | Int32 | The index of value field in the value region. |
| type | PivotFilterType | The type of filtering data. |
| value1 | Double | The value of filter condition |
| value2 | Double | The upper-bound value of between filter condition |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotFieldMethodFilterByValueWithInt32PivotFilterTypeDoubleDoubDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Product";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B1"].Value = "Price";
worksheet.Cells["B2"].Value = 2.5;
worksheet.Cells["B3"].Value = 1.8;
worksheet.Cells["B4"].Value = 3.2;
worksheet.Cells["C1"].Value = "Quantity";
worksheet.Cells["C2"].Value = 100;
worksheet.Cells["C3"].Value = 150;
worksheet.Cells["C4"].Value = 80;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
// Add data fields
pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Get the pivot field
PivotField pivotField = pivotTable.RowFields[0];
try
{
// Call FilterByValue method with parameters (Int32, PivotFilterType, Double, Double)
// Filter products where Quantity (field index 1) is between 90 and 160
PivotFilter filter = pivotField.FilterByValue(1, PivotFilterType.ValueBetween, 90.0, 160.0);
Console.WriteLine("FilterByValue method executed successfully");
Console.WriteLine($"Filter type: {filter.FilterType}");
Console.WriteLine($"Value field index: {filter.ValueFieldIndex}");
// Refresh pivot table to show changes
pivotTable.RefreshData();
pivotTable.CalculateData();
}
catch (Exception ex)
{
Console.WriteLine($"Error executing FilterByValue method: {ex.Message}");
}
// Save the result
workbook.Save("PivotFieldMethodFilterByValueDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
