##UnionRange.Union
UnionRange method. Union another range
## Union(string) {#union_2}
Union another range.
```csharp
public UnionRange Union(string range)
```
| Parameter | Type | Description |
| --- | --- | --- |
| range | String | The range. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class UnionRangeMethodUnionWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create initial range and populate with data
Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
range1[0, 0].PutValue("Range1");
range1[0, 1].PutValue(100);
range1[1, 0].PutValue("Data");
range1[1, 1].PutValue(200);
// Create UnionRange from the initial range
UnionRange unionRange = worksheet.Cells.CreateRange(range1.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range1 });
try
{
// Call the Union method with a string parameter representing another range
UnionRange combinedRange = unionRange.Union("C1:D2");
// Populate the second range with data
worksheet.Cells["C1"].PutValue("Range2");
worksheet.Cells["D1"].PutValue(300);
worksheet.Cells["C2"].PutValue("More");
worksheet.Cells["D2"].PutValue(400);
Console.WriteLine("Union method executed successfully with parameter (String)");
Console.WriteLine($"Combined range refers to: {combinedRange.RefersTo}");
Console.WriteLine($"Total ranges in union: {combinedRange.RangeCount}");
// Display information about the combined range
Console.WriteLine("\nCombined Range Info:");
Console.WriteLine($"FirstRow: {combinedRange.FirstRow}, FirstColumn: {combinedRange.FirstColumn}");
Console.WriteLine($"RowCount: {combinedRange.RowCount}, ColumnCount: {combinedRange.ColumnCount}");
Console.WriteLine($"CellCount: {combinedRange.CellCount}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Union method: {ex.Message}");
}
// Save the workbook
workbook.Save("UnionRangeMethodUnionWithStringDemo.xlsx");
}
}
}
```
### See Also
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Union(UnionRange) {#union_1}
Union another range.
```csharp
public UnionRange Union(UnionRange unionRange)
```
| Parameter | Type | Description |
| --- | --- | --- |
| unionRange | UnionRange | The range. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class UnionRangeMethodUnionWithUnionRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create first range and populate with data
Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
range1[0, 0].PutValue("Range1");
range1[0, 1].PutValue(100);
range1[1, 0].PutValue("Data");
range1[1, 1].PutValue(200);
// Create second range and populate with data
Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C1:D2");
range2[0, 0].PutValue("Range2");
range2[0, 1].PutValue(300);
range2[1, 0].PutValue("More");
range2[1, 1].PutValue(400);
// Create UnionRange from the first range
UnionRange unionRange1 = worksheet.Cells.CreateRange(range1.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range1 });
// Create UnionRange from the second range
UnionRange unionRange2 = worksheet.Cells.CreateRange(range2.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range2 });
try
{
// Call the Union method with UnionRange parameter
UnionRange combinedRange = unionRange1.Union(unionRange2);
Console.WriteLine("Union method executed successfully with parameter (UnionRange)");
Console.WriteLine($"Combined range refers to: {combinedRange.RefersTo}");
Console.WriteLine($"Total ranges in union: {combinedRange.RangeCount}");
// Display information about the combined range
Console.WriteLine("\nCombined Range Info:");
Console.WriteLine($"FirstRow: {combinedRange.FirstRow}, FirstColumn: {combinedRange.FirstColumn}");
Console.WriteLine($"RowCount: {combinedRange.RowCount}, ColumnCount: {combinedRange.ColumnCount}");
Console.WriteLine($"CellCount: {combinedRange.CellCount}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Union method: {ex.Message}");
}
// Save the workbook
workbook.Save("UnionRangeMethodUnionWithUnionRangeDemo.xlsx");
}
}
}
```
### See Also
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Union(Range[]) {#union}
Union the ranges.
```csharp
public UnionRange Union(Range[] ranges)
```
| Parameter | Type | Description |
| --- | --- | --- |
| ranges | Range[] | The ranges. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class UnionRangeMethodUnionWithRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample ranges to demonstrate union
Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C3:D4");
Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("E5:F6");
// Put values in the ranges to visualize them
range1[0, 0].PutValue("Range1");
range2[0, 0].PutValue("Range2");
range3[0, 0].PutValue("Range3");
try
{
// Create initial union range
UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range1 });
// Call the Union method with Range[] parameter
Aspose.Cells.Range[] rangesToUnion = new Aspose.Cells.Range[] { range2, range3 };
UnionRange resultUnion = unionRange.Union(rangesToUnion);
Console.WriteLine("Union method executed successfully with parameters (Range[])");
Console.WriteLine($"Resulting union range count: {resultUnion.RangeCount}");
Console.WriteLine($"Resulting union refers to: {resultUnion.RefersTo}");
// Highlight the union result by setting background color
Style highlightStyle = workbook.CreateStyle();
highlightStyle.ForegroundColor = System.Drawing.Color.LightYellow;
highlightStyle.Pattern = BackgroundType.Solid;
resultUnion.SetStyle(highlightStyle);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Union method: {ex.Message}");
}
// Save the result
workbook.Save("UnionRangeMethodUnionWithRangeDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../../range/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
