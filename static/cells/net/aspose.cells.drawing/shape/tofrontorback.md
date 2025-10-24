##Shape.ToFrontOrBack
Shape method. Brings the shape to the front or sends the shape to back
## Shape.ToFrontOrBack method
Brings the shape to the front or sends the shape to back.
```csharp
public void ToFrontOrBack(int orders)
```
| Parameter | Type | Description |
| --- | --- | --- |
| orders | Int32 | If it's less than zero, sets the shape to back. If it's greater than zero, brings the shape to front. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeMethodToFrontOrBackWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add two shapes to demonstrate z-order
Aspose.Cells.Drawing.Shape shape1 = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
Aspose.Cells.Drawing.Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);
// Move shape2 2 positions forward in z-order
shape2.ToFrontOrBack(2);
// Move shape1 1 position backward in z-order
shape1.ToFrontOrBack(-1);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
