##Shape.ThreeDFormat
Shape property. Gets and sets 3d format of the shape
## Shape.ThreeDFormat property
Gets and sets 3d format of the shape.
```csharp
public ThreeDFormat ThreeDFormat { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyThreeDFormatDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);
// Access and modify 3D format properties
ThreeDFormat threeDFormat = shape.ThreeDFormat;
threeDFormat.ExtrusionColor.Color = System.Drawing.Color.Blue;
threeDFormat.LightAngle = 45;
threeDFormat.ContourWidth = 2;
threeDFormat.ContourColor.Color = System.Drawing.Color.Red;
// Save the workbook
workbook.Save("ThreeDFormatDemo.xlsx");
}
}
}
```
### See Also
* class [ThreeDFormat](../../threedformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
