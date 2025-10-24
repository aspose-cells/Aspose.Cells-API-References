##Shape.LowerRightRow
Shape property. Represents lower right corner row index
## Shape.LowerRightRow property
Represents lower right corner row index.
```csharp
public int LowerRightRow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyLowerRightRowDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
// Set and demonstrate LowerRightRow property
Console.WriteLine("Original LowerRightRow: " + shape.LowerRightRow);
shape.LowerRightRow = 3;
Console.WriteLine("Modified LowerRightRow: " + shape.LowerRightRow);
// Conditional modification as per test case
if (shape.LowerRightRow == 3)
{
shape.LowerRightRow = 1;
Console.WriteLine("Final LowerRightRow after condition: " + shape.LowerRightRow);
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
