##Range.IsIntersect
Range method. Indicates whether the range is intersect
## Range.IsIntersect method
Indicates whether the range is intersect.
```csharp
public bool IsIntersect(Range range)
```
| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The range. |
### Return Value
Whether the range is intersect.
### Remarks
If the two ranges area not in the same worksheet ,return false.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class RangeMethodIsIntersectWithRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create two ranges to test intersection
Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B5");
Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B3:D8");
Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("C10:D15");
try
{
// Check if range1 intersects with range2 (should intersect)
bool result1 = range1.IsIntersect(range2);
Console.WriteLine($"Range A1:B5 intersects with B3:D8: {result1}");
// Check if range1 intersects with range3 (should not intersect)
bool result2 = range1.IsIntersect(range3);
Console.WriteLine($"Range A1:B5 intersects with C10:D15: {result2}");
// Fill the ranges with different colors to visualize them
Style style1 = workbook.CreateStyle();
style1.ForegroundColor = System.Drawing.Color.LightBlue;
style1.Pattern = BackgroundType.Solid;
range1.SetStyle(style1);
Style style2 = workbook.CreateStyle();
style2.ForegroundColor = System.Drawing.Color.LightGreen;
style2.Pattern = BackgroundType.Solid;
range2.SetStyle(style2);
Style style3 = workbook.CreateStyle();
style3.ForegroundColor = System.Drawing.Color.LightPink;
style3.Pattern = BackgroundType.Solid;
range3.SetStyle(style3);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing IsIntersect method: {ex.Message}");
}
// Save the workbook
workbook.Save("RangeMethodIsIntersectWithRangeDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
