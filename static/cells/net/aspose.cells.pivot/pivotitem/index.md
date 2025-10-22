##PivotItem.Index
PivotItem property. Gets the index of the pivot item in cache field
## PivotItem.Index property
Gets the index of the pivot item in cache field.
```csharp
public int Index { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotItemPropertyIndexDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["B2"].Value = 10;
cells["A3"].Value = "Orange";
cells["B3"].Value = 15;
cells["A4"].Value = "Banana";
cells["B4"].Value = 20;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Get the row field
PivotField rowField = pivotTable.RowFields[0];
// Access pivot items using Index property
foreach (PivotItem item in rowField.PivotItems)
{
Console.WriteLine($"Item: {item.Value}, Index: {item.Index}");
// Hide item detail using Index property
if (item.Value.ToString() == "Apple")
{
rowField.HideItemDetail(item.Index, true);
}
}
// Calculate and refresh pivot table
pivotTable.CalculateData();
pivotTable.RefreshData();
// Save the workbook
workbook.Save("PivotItemPropertyIndexDemo_out.xlsx");
}
}
}
```
### See Also
* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
