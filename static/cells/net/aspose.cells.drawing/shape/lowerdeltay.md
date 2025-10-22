##Shape.LowerDeltaY
Shape property. Gets or sets the shapes vertical offset from its lower right corner row
## Shape.LowerDeltaY property
Gets or sets the shape's vertical offset from its lower right corner row.
```csharp
public int LowerDeltaY { get; set; }
```
### Remarks
The range of value is 0 to 256.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyLowerDeltaYDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample shape with correct parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
// Set and demonstrate LowerDeltaY property
shape.LowerDeltaY = 20;
Console.WriteLine("Initial LowerDeltaY: " + shape.LowerDeltaY);
// Modify LowerDeltaY conditionally
if (shape.LowerDeltaY == 20)
{
shape.LowerDeltaY = 10;
Console.WriteLine("Modified LowerDeltaY: " + shape.LowerDeltaY);
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
