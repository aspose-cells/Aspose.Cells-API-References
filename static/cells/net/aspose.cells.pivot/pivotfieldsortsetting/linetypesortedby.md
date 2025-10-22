##PivotFieldSortSetting.LineTypeSortedBy
PivotFieldSortSetting property. The pivot line type sorted by
## PivotFieldSortSetting.LineTypeSortedBy property
The pivot line type sorted by.
```csharp
public PivotLineType LineTypeSortedBy { get; }
```
### Remarks
Only works when not sorting this field by labels.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldSortSettingPropertyLineTypeSortedByDemo
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
cells["B3"].Value = 15;
cells["B4"].Value = 5;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
// Sort by ascending order with line type - provide empty string for cellName parameter
pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.GrandTotal, "");
// Demonstrate LineTypeSortedBy property
Console.WriteLine("LineTypeSortedBy: " + pivotTable.RowFields[0].SortSetting.LineTypeSortedBy);
// Change sort to use regular line type
pivotTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "C5");
Console.WriteLine("LineTypeSortedBy after change: " + pivotTable.RowFields[0].SortSetting.LineTypeSortedBy);
}
}
}
```
### See Also
* enum [PivotLineType](../../pivotlinetype/)
* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
