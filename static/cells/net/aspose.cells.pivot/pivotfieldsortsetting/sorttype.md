##PivotFieldSortSetting.SortType
PivotFieldSortSetting property. Represents the SortOrder
## PivotFieldSortSetting.SortType property
Represents the [`SortOrder`](../../../aspose.cells/sortorder/).
```csharp
public SortOrder SortType { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldSortSettingPropertySortTypeDemo
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
worksheet.Cells["B3"].Value = 200;
worksheet.Cells["B4"].Value = 150;
// Create pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
// Sort the row field in ascending order
pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "E5");
// Demonstrate SortType property
Console.WriteLine("Sort Type: " + pivotTable.RowFields[0].SortSetting.SortType);
Console.WriteLine("Sorted by cell: " + pivotTable.RowFields[0].SortSetting.Cell);
// Change sort order and demonstrate again
pivotTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "E6");
Console.WriteLine("Updated Sort Type: " + pivotTable.RowFields[0].SortSetting.SortType);
Console.WriteLine("Updated sorted by cell: " + pivotTable.RowFields[0].SortSetting.Cell);
}
}
}
```
### See Also
* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
