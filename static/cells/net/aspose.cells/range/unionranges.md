##Range.UnionRanges
Range method. Returns the union result of two ranges
## Range.UnionRanges method
Returns the union result of two ranges.
```csharp
public UnionRange UnionRanges(Range[] ranges)
```
| Parameter | Type | Description |
| --- | --- | --- |
| ranges | Range[] | The range |
### Return Value
The union of two ranges.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class RangeMethodUnionRangesWithRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data in cells
worksheet.Cells["A1"].PutValue("Range 1");
worksheet.Cells["B1"].PutValue("Data 1");
worksheet.Cells["C1"].PutValue("Data 2");
worksheet.Cells["A5"].PutValue("Range 2");
worksheet.Cells["B5"].PutValue("Data 3");
worksheet.Cells["C5"].PutValue("Data 4");
// Create ranges to union
Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:C3");
Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A5:C7");
try
{
// Call UnionRanges with Range[] parameter
Aspose.Cells.Range[] rangesToUnion = new Aspose.Cells.Range[] { range1, range2 };
UnionRange unionRange = range1.UnionRanges(rangesToUnion);
// Apply style to show the union range
Style style = workbook.CreateStyle();
style.BackgroundColor = System.Drawing.Color.LightBlue;
unionRange.ApplyStyle(style, new StyleFlag { All = true });
Console.WriteLine($"Union range created successfully. Address: {unionRange.RefersTo}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing UnionRanges method: {ex.Message}");
}
// Save the result
workbook.Save("UnionRangesDemo.xlsx");
}
}
}
```
### See Also
* class [UnionRange](../../unionrange/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
