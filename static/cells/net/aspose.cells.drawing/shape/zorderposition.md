##Shape.ZOrderPosition
Shape property. Returns the position of a shape in the zorder
## Shape.ZOrderPosition property
Returns the position of a shape in the z-order.
```csharp
public int ZOrderPosition { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyZOrderPositionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add three shapes to demonstrate ZOrder
Shape shape1 = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);
Shape shape3 = worksheet.Shapes.AddRectangle(90, 90, 100, 100, 0, 0);
// Set ZOrder positions
shape1.ZOrderPosition = 0;
shape2.ZOrderPosition = 1;
shape3.ZOrderPosition = 2;
// Change ZOrder of shape3 to bring it to front
shape3.ZOrderPosition = 0;
// Save the workbook
workbook.Save("ShapeZOrderDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
