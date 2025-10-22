##Shape.WidthInShape
Shape property. Represents the width of the shape in unit of 1/4000 of the parent shape
## Shape.WidthInShape property
Represents the width of the shape, in unit of 1/4000 of the parent shape.
```csharp
public int WidthInShape { get; set; }
```
### Remarks
Only Applies when this shape in the group or chart.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyWidthInShapeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create two rectangle shapes
Shape rect1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
Shape rect2 = worksheet.Shapes.AddRectangle(0, 100, 0, 0, 100, 100);
// Group the shapes using shape objects
GroupShape group = worksheet.Shapes.Group(new Shape[] { rect1, rect2 });
// Demonstrate WidthInShape usage
if (rect1.IsInGroup && rect1.WidthInShape == 2000)
{
rect1.WidthInShape = 4000;
}
// Save modified workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
