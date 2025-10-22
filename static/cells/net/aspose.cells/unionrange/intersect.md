##UnionRange.Intersect
UnionRange method. Intersects another range
## Intersect(string) {#intersect_2}
Intersects another range.
```csharp
public UnionRange Intersect(string range)
```
| Parameter | Type | Description |
| --- | --- | --- |
| range | String | The range. |
### Remarks
If the two union ranges are not intersected, returns null.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class UnionRangeMethodIntersectWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some sample data
worksheet.Cells["A1"].PutValue("A1");
worksheet.Cells["B1"].PutValue("B1");
worksheet.Cells["A2"].PutValue("A2");
worksheet.Cells["B2"].PutValue("B2");
// Create a UnionRange covering A1:B2
UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });
try
{
// Call Intersect with a string parameter representing range A1:A2
UnionRange intersectionResult = unionRange.Intersect("A1:A2");
// Display information about the intersection
Console.WriteLine($"Intersection result range: {intersectionResult.RefersTo}");
Console.WriteLine($"First row: {intersectionResult.FirstRow}");
Console.WriteLine($"First column: {intersectionResult.FirstColumn}");
Console.WriteLine($"Row count: {intersectionResult.RowCount}");
Console.WriteLine($"Column count: {intersectionResult.ColumnCount}");
// Highlight the intersection area
Style highlightStyle = workbook.CreateStyle();
highlightStyle.BackgroundColor = System.Drawing.Color.LightGreen;
intersectionResult.SetStyle(highlightStyle);
Console.WriteLine("Intersect method executed successfully with parameter (String)");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Intersect method: {ex.Message}");
}
// Save the result
workbook.Save("UnionRangeMethodIntersectWithStringDemo.xlsx");
}
}
}
```
### See Also
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Intersect(UnionRange) {#intersect_1}
Intersects another range.
```csharp
public UnionRange Intersect(UnionRange unionRange)
```
| Parameter | Type | Description |
| --- | --- | --- |
| unionRange | UnionRange | The range. |
### Remarks
If the two union ranges are not intersected, returns null.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class UnionRangeMethodIntersectWithUnionRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some data in cells
worksheet.Cells["A1"].PutValue("A1");
worksheet.Cells["B1"].PutValue("B1");
worksheet.Cells["C1"].PutValue("C1");
worksheet.Cells["A2"].PutValue("A2");
worksheet.Cells["B2"].PutValue("B2");
worksheet.Cells["C2"].PutValue("C2");
// Create two union ranges
UnionRange range1 = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });
UnionRange range2 = worksheet.Cells.CreateRange("B1:C2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("B1:C2") });
try
{
// Call the Intersect method with UnionRange parameter
UnionRange intersectionResult = range1.Intersect(range2);
// Display information about the intersection
Console.WriteLine($"Intersection result range: {intersectionResult.RefersTo}");
Console.WriteLine($"First row: {intersectionResult.FirstRow}");
Console.WriteLine($"First column: {intersectionResult.FirstColumn}");
Console.WriteLine($"Row count: {intersectionResult.RowCount}");
Console.WriteLine($"Column count: {intersectionResult.ColumnCount}");
// Highlight the intersection area
Style highlightStyle = workbook.CreateStyle();
highlightStyle.BackgroundColor = System.Drawing.Color.Yellow;
intersectionResult.SetStyle(highlightStyle);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Intersect method: {ex.Message}");
}
// Save the workbook
workbook.Save("UnionRangeMethodIntersectWithUnionRangeDemo.xlsx");
}
}
}
```
### See Also
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Intersect(Range[]) {#intersect}
Intersects another range.
```csharp
public UnionRange Intersect(Range[] ranges)
```
| Parameter | Type | Description |
| --- | --- | --- |
| ranges | Range[] | The range. |
### Remarks
If the two union ranges are not intersected, returns null.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class UnionRangeMethodIntersectWithRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data in cells
worksheet.Cells["A1"].PutValue("A1");
worksheet.Cells["B1"].PutValue("B1");
worksheet.Cells["A2"].PutValue("A2");
worksheet.Cells["B2"].PutValue("B2");
// Create ranges to intersect
Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B1");
Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A1:A2");
Aspose.Cells.Range[] rangesToIntersect = new Aspose.Cells.Range[] { range1, range2 };
// Get the union range of the worksheet
UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });
try
{
// Call the Intersect method with Range[] parameter
UnionRange intersectionResult = unionRange.Intersect(rangesToIntersect);
// Display information about the intersection result
Console.WriteLine($"Intersection result range: {intersectionResult.RefersTo}");
Console.WriteLine($"First row: {intersectionResult.FirstRow}");
Console.WriteLine($"First column: {intersectionResult.FirstColumn}");
Console.WriteLine($"Row count: {intersectionResult.RowCount}");
Console.WriteLine($"Column count: {intersectionResult.ColumnCount}");
// Highlight the intersection area
Style style = workbook.CreateStyle();
style.BackgroundColor = System.Drawing.Color.Yellow;
intersectionResult.SetStyle(style);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Intersect method: {ex.Message}");
}
// Save the result
workbook.Save("UnionRangeMethodIntersectWithRangeDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../../range/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
