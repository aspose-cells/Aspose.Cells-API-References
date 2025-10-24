##Shape.UpperDeltaY
Shape property. Gets or sets the shapes vertical offset from its upper left corner row
## Shape.UpperDeltaY property
Gets or sets the shape's vertical offset from its upper left corner row.
```csharp
public int UpperDeltaY { get; set; }
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
public class ShapePropertyUpperDeltaYDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate UpperDeltaY property
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
// Set and display initial UpperDeltaY value
shape.UpperDeltaY = 3;
Console.WriteLine("Initial UpperDeltaY: " + shape.UpperDeltaY);
// Modify UpperDeltaY value
if (shape.UpperDeltaY == 3)
{
shape.UpperDeltaY = 1;
Console.WriteLine("Modified UpperDeltaY: " + shape.UpperDeltaY);
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
