##Range.Left
Range property. Gets the distance in points from the left edge of column A to the left edge of the range
## Range.Left property
Gets the distance, in points, from the left edge of column A to the left edge of the range.
```csharp
public double Left { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangePropertyLeftDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a range from B2 to C4
Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
// Demonstrate Left property usage
Console.WriteLine("Range Left position: " + range.Left);
Console.WriteLine("Range Width: " + range.Width);
// Calculate expected values based on test case
double expectedLeft = 64 / 96.0 * 72;
Console.WriteLine("Expected Left position: " + expectedLeft);
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
