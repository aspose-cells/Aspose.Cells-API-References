##Shape.AnchorType
Shape property. Gets and set the type of the shape anchor placeholder
## Shape.AnchorType property
Gets and set the type of the shape anchor placeholder.
```csharp
public ShapeAnchorType AnchorType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyAnchorTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape with default anchor type
Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 0, 0);
// Check and modify anchor type
if (shape.AnchorType == ShapeAnchorType.OneCellAnchor)
{
shape.AnchorType = ShapeAnchorType.TwoCellAnchor;
Console.WriteLine("Anchor type changed to TwoCellAnchor");
}
// Save the workbook
workbook.Save("ShapeAnchorTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [ShapeAnchorType](../../shapeanchortype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
