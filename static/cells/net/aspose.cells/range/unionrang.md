##Range.UnionRang
Range method. Returns the union result of two ranges
## Range.UnionRang method
Returns the union result of two ranges.
```csharp
[Obsolete("Use Range.UnionRanges() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Range[] UnionRang(Range range)
```
| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The range |
### Return Value
The union of two ranges.
### Remarks
NOTE: This method is now obsolete. Instead, please use Range.UnionRanges() method. This method will be removed 12 months later since May 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using Range = Aspose.Cells.Range; // Add this alias to resolve ambiguity
public class RangeMethodUnionRangWithRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create two ranges to demonstrate UnionRang
Range range1 = worksheet.Cells.CreateRange("A1:B2");
Range range2 = worksheet.Cells.CreateRange("C3:D4");
// Set some values in the ranges for visualization
range1[0, 0].PutValue("Range1");
range1[1, 1].PutValue("Data");
range2[0, 0].PutValue("Range2");
range2[1, 1].PutValue("Data");
try
{
// Call the UnionRang method to combine the two ranges
Range[] unionResult = range1.UnionRang(range2);
// Display information about the union result
Console.WriteLine("UnionRang method executed successfully.");
Console.WriteLine($"Number of ranges in union: {unionResult.Length}");
Console.WriteLine($"First union range address: {unionResult[0].Address}");
Console.WriteLine($"Second union range address: {unionResult[1].Address}");
// Mark the union ranges with a border for visualization
foreach (Range r in unionResult)
{
r.SetOutlineBorders(CellBorderType.Thin, System.Drawing.Color.Black);
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing UnionRang method: {ex.Message}");
}
// Save the result
workbook.Save("RangeMethodUnionRangWithRangeDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
