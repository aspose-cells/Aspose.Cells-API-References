##UnionRange.FirstColumn
UnionRange property. Gets the index of the first column of the range
## UnionRange.FirstColumn property
Gets the index of the first column of the range.
```csharp
public int FirstColumn { get; }
```
### Remarks
Only effects when it only contains one range.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class UnionRangePropertyFirstColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some data
worksheet.Cells["A1"].PutValue("Header1");
worksheet.Cells["B1"].PutValue("Header2");
worksheet.Cells["C1"].PutValue("Header3");
worksheet.Cells["A2"].PutValue("Data1");
worksheet.Cells["B2"].PutValue("Data2");
worksheet.Cells["C2"].PutValue("Data3");
// Create a union range
Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:C1");
Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A2:C2");
UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });
// Display the FirstColumn property
Console.WriteLine("First column index of the union range: " + unionRange.FirstColumn);
// Demonstrate usage of FirstColumn in operations
Console.WriteLine("First column name: " + CellsHelper.ColumnIndexToName(unionRange.FirstColumn));
// Apply formatting to the first column of the union range
Style style = workbook.CreateStyle();
style.Font.IsBold = true;
style.ForegroundColor = System.Drawing.Color.LightGray;
style.Pattern = BackgroundType.Solid;
Aspose.Cells.Range firstColumnRange = worksheet.Cells.CreateRange(
unionRange.FirstRow, unionRange.FirstColumn,
unionRange.RowCount, 1);
firstColumnRange.ApplyStyle(style, new StyleFlag { FontBold = true, CellShading = true });
// Save the result
workbook.Save("UnionRangePropertyFirstColumnDemo.xlsx");
}
}
}
```
### See Also
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
