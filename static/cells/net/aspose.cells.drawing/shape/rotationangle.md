##Shape.RotationAngle
Shape property. Gets and sets the rotation of the shape
## Shape.RotationAngle property
Gets and sets the rotation of the shape.
```csharp
public double RotationAngle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyRotationAngleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 100, 200, 0, 0);
// Set rotation angle to 60 degrees
shape.RotationAngle = 60;
Console.WriteLine("Shape rotation angle set to: " + shape.RotationAngle);
// Get current rotation angle
double currentAngle = shape.RotationAngle;
Console.WriteLine("Current shape rotation angle: " + currentAngle);
// Save the workbook
workbook.Save("ShapeRotationDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
