##PivotFieldSortSetting.Cell
PivotFieldSortSetting property. Sorts by the values in which row or column
## PivotFieldSortSetting.Cell property
Sorts by the values in which row or column.
```csharp
public string Cell { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldSortSettingPropertyCellDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["A3"].Value = "Orange";
cells["A4"].Value = "Banana";
cells["B2"].Value = 10;
cells["B3"].Value = 5;
cells["B4"].Value = 8;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Sort by cell reference
pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "A2");
// Demonstrate Cell property usage
Console.WriteLine("Sorting by cell: " + pivotTable.RowFields[0].SortSetting.Cell);
// Change sort cell
pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "A3");
Console.WriteLine("Changed sort cell to: " + pivotTable.RowFields[0].SortSetting.Cell);
// Clear cell sorting
pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.GrandTotal, "");
Console.WriteLine("After clearing cell sort: " +
(string.IsNullOrEmpty(pivotTable.RowFields[0].SortSetting.Cell) ? "Empty" : "Has value"));
}
}
}
```
### See Also
* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
