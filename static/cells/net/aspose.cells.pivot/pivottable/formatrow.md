##PivotTable.FormatRow
PivotTable method. Format the row data in the pivottable area
## PivotTable.FormatRow method
Format the row data in the pivottable area
```csharp
public void FormatRow(int row, Style style)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row Index of the Row object |
| style | Style | Style which is to format |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodFormatRowWithInt32StyleDemo
{
public static void Run()
{
// Create a workbook
Workbook wb = new Workbook();
Worksheet worksheet = wb.Worksheets[0];
// Sample data for pivot table
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["A4"].PutValue("A");
worksheet.Cells["B4"].PutValue(30);
worksheet.Cells["A5"].PutValue("B");
worksheet.Cells["B5"].PutValue(40);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
// Create style for formatting
Style style = wb.CreateStyle();
style.Custom = "0.00%";
style.Font.Name = "Calibri";
style.Font.Size = 11;
// Find and format rows
Cell cell = worksheet.Cells.Find("A", null);
if (cell != null)
{
pivotTable.FormatRow(cell.Row, style);
}
cell = worksheet.Cells.Find("B", null);
if (cell != null)
{
pivotTable.FormatRow(cell.Row, style);
}
// Save the workbook
wb.Save("PivotTableFormatRowDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
