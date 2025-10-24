##UnionRange.FirstRow
UnionRange property. Gets the index of the first row of the range
## UnionRange.FirstRow property
Gets the index of the first row of the range.
```csharp
public int FirstRow { get; }
```
### Remarks
Only effects when it only contains one range.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class UnionRangePropertyFirstRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate sample data
for (int row = 0; row < 10; row++)
{
for (int col = 0; col < 5; col++)
{
worksheet.Cells[row, col].Value = $"Row {row}, Col {col}";
}
}
// Create a union range from A2:C5 and A7:C9
Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A2:C5");
Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A7:C9");
UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });
// Display FirstRow property
Console.WriteLine("FirstRow of union range: " + unionRange.FirstRow);
// Demonstrate usage by highlighting the first row
Style highlightStyle = workbook.CreateStyle();
highlightStyle.Font.IsBold = true;
highlightStyle.ForegroundColor = System.Drawing.Color.LightGreen;
highlightStyle.Pattern = BackgroundType.Solid;
Aspose.Cells.Range firstRowRange = worksheet.Cells.CreateRange(
unionRange.FirstRow,
unionRange.FirstColumn,
1,
unionRange.ColumnCount);
firstRowRange.ApplyStyle(highlightStyle, new StyleFlag { FontBold = true, CellShading = true });
// Create another range and compare FirstRow values
Aspose.Cells.Range singleRange = worksheet.Cells.CreateRange("D1:F5");
Console.WriteLine("FirstRow of single range: " + singleRange.FirstRow);
Console.WriteLine("Is union range starting after single range? " +
(unionRange.FirstRow > singleRange.FirstRow));
// Save the workbook
workbook.Save("UnionRangeFirstRowDemo.xlsx");
}
}
}
```
### See Also
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
