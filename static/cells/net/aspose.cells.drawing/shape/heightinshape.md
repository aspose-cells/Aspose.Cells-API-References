##Shape.HeightInShape
Shape property. Represents the vertical offset of shape from the top border of the parent shape in unit of 1/4000 of height of the parent shape
## Shape.HeightInShape property
Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape..
```csharp
public int HeightInShape { get; set; }
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
public class ShapePropertyHeightInShapeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add shapes first with all required parameters
Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 10, 10);
Shape oval = worksheet.Shapes.AddOval(0, 0, 100, 100, 10, 120);
// Group the shapes
Shape[] shapes = { rectangle, oval };
GroupShape groupShape = worksheet.Shapes.Group(shapes);
// Set the height of the rectangle relative to the parent group shape (1/4000 of parent height)
rectangle.HeightInShape = 2000; // Half the height of the parent
oval.HeightInShape = 4000; // Full height of the parent
// Save the workbook
workbook.Save("ShapeHeightInShapeDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
