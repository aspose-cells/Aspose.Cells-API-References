##Range.Height
Range property. Gets the width of a range in points
## Range.Height property
Gets the width of a range in points.
```csharp
public double Height { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangePropertyHeightDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set row heights for demonstration
worksheet.Cells.SetRowHeight(1, 15.0); // Row 2 (0-based index 1)
worksheet.Cells.SetRowHeight(2, 20.0); // Row 3
worksheet.Cells.SetRowHeight(3, 25.0); // Row 4
// Create a range spanning rows 2-4 (B2:C4)
Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
// Demonstrate Height property
Console.WriteLine("Range Height: " + range.Height);
Console.WriteLine("Calculated Height (sum of row heights): " +
(worksheet.Cells.GetRowHeight(1) +
worksheet.Cells.GetRowHeight(2) +
worksheet.Cells.GetRowHeight(3)));
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
