##PivotField.SortSetting
PivotField property. Gets all settings of auto sorting
## PivotField.SortSetting property
Gets all settings of auto sorting
```csharp
public PivotFieldSortSetting SortSetting { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertySortSettingDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 100;
worksheet.Cells["B3"].Value = 50;
worksheet.Cells["B4"].Value = 75;
// Create pivot table
int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
PivotField rowField = pivotTable.RowFields[0];
// Demonstrate SortSetting property
rowField.SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "C5");
Console.WriteLine("Sort Type: " + rowField.SortSetting.SortType);
Console.WriteLine("Sorted by Cell: " + rowField.SortSetting.Cell);
Console.WriteLine("Line Type Sorted By: " + rowField.SortSetting.LineTypeSortedBy);
// Change sort settings
rowField.SortBy(SortOrder.Descending, 0, PivotLineType.GrandTotal, null);
Console.WriteLine("\nAfter changing sort settings:");
Console.WriteLine("Sort Type: " + rowField.SortSetting.SortType);
Console.WriteLine("Sorted by Cell: " + (string.IsNullOrEmpty(rowField.SortSetting.Cell) ? "null" : rowField.SortSetting.Cell));
Console.WriteLine("Line Type Sorted By: " + rowField.SortSetting.LineTypeSortedBy);
}
}
}
```
### See Also
* class [PivotFieldSortSetting](../../pivotfieldsortsetting/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
