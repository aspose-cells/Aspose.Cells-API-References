##Range.Width
Range property. Gets the width of a range in points
## Range.Width property
Gets the width of a range in points.
```csharp
public double Width { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangePropertyWidthDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set column widths to demonstrate Width property
worksheet.Cells.SetColumnWidth(1, 20); // Column B width = 20
worksheet.Cells.SetColumnWidth(2, 30); // Column C width = 30
Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
// Display range width (sum of column widths in the range)
Console.WriteLine("Range Width: " + range.Width);
// Display individual properties for verification
Console.WriteLine("Range Left Position: " + range.Left);
Console.WriteLine("Range Top Position: " + range.Top);
Console.WriteLine("Range Height: " + range.Height);
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
