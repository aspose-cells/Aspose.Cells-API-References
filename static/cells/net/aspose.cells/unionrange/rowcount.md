##UnionRange.RowCount
UnionRange property. Gets the count of rows in the range
## UnionRange.RowCount property
Gets the count of rows in the range.
```csharp
public int RowCount { get; }
```
### Remarks
Only effects when it only contains one range.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class UnionRangePropertyRowCountDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate data in the worksheet
for (int row = 0; row < 10; row++)
{
for (int col = 0; col < 5; col++)
{
worksheet.Cells[row, col].Value = $"Data {row},{col}";
}
}
// Create a union range from A1 to E5
Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:E5");
Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A6:E10");
UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });
// Display RowCount property
Console.WriteLine("RowCount of union range: " + unionRange.RowCount);
// Demonstrate usage by iterating through rows
for (int i = 0; i < unionRange.RowCount; i++)
{
Aspose.Cells.Range currentRow = worksheet.Cells.CreateRange(
unionRange.FirstRow + i,
unionRange.FirstColumn,
1,
unionRange.ColumnCount);
Console.WriteLine($"Row {i + 1} first cell value: " + currentRow[0, 0].Value);
}
// Create a new range with different row count
Aspose.Cells.Range newRange = worksheet.Cells.CreateRange("A1:E3");
Console.WriteLine("RowCount of new range: " + newRange.RowCount);
// Apply formatting based on row count
Style style = workbook.CreateStyle();
style.Font.IsBold = true;
style.ForegroundColor = System.Drawing.Color.LightYellow;
style.Pattern = BackgroundType.Solid;
for (int i = 0; i < unionRange.RowCount; i += 2)
{
Aspose.Cells.Range rowRange = worksheet.Cells.CreateRange(
unionRange.FirstRow + i,
unionRange.FirstColumn,
1,
unionRange.ColumnCount);
rowRange.ApplyStyle(style, new StyleFlag { FontBold = true, CellShading = true });
}
// Save the workbook
workbook.Save("UnionRangeRowCountDemo.xlsx");
}
}
}
```
### See Also
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
