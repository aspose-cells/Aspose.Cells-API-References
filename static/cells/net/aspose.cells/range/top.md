##Range.Top
Range property. Gets the distance in points from the top edge of row 1 to the top edge of the range
## Range.Top property
Gets the distance, in points, from the top edge of row 1 to the top edge of the range.
```csharp
public double Top { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangePropertyTopDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a range and set some values
Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
range[0, 0].PutValue("Test");
// Demonstrate Top property usage
Console.WriteLine("Range Top position: " + range.Top);
Console.WriteLine("Range Height: " + range.Height);
Console.WriteLine("Range Left position: " + range.Left);
Console.WriteLine("Range Width: " + range.Width);
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
