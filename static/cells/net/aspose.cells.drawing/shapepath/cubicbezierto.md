##ShapePath.CubicBezierTo
ShapePath method. Appends a cubic Bézier curve to the current figure. The starting point is the end point of the current figure.Unit Pixel
## ShapePath.CubicBezierTo method
Appends a cubic Bézier curve to the current figure. The starting point is the end point of the current figure.Unit: Pixel.
```csharp
public void CubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX,
float endY)
```
| Parameter | Type | Description |
| --- | --- | --- |
| ctrX1 | Single | The x-coordinate of the first control point for the curve(Unit: Pixel). |
| ctrY1 | Single | The y-coordinate of the first control point for the curve(Unit: Pixel). |
| ctrX2 | Single | The x-coordinate of the second control point for the curve(Unit: Pixel). |
| ctrY2 | Single | The y-coordinate of the second control point for the curve(Unit: Pixel). |
| endX | Single | The x-coordinate of the endpoint of the curve(Unit: Pixel). |
| endY | Single | The y-coordinate of the endpoint of the curve(Unit: Pixel). |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ShapePathMethodCubicBezierToWithSingleSingleSingleSingleSingleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
//Create a new shape path
ShapePath shapePath1 = new ShapePath();
shapePath1.MoveTo(0, 0);
shapePath1.CubicBezierTo(48.24997f, 0.6844f,
96.5f, -7.148871f,
130, 11.517795f);
shapePath1.CubicBezierTo(163.5f, 30.18446f,
182.24997f, 75.351f,
201, 120.517795f);
shapePath1.MoveTo(150, 70);
shapePath1.ArcTo(25, 25, 0, 270);
//add free form
worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath1 });
// Save the result
workbook.Save("ShapePathMethodCubicBezierToDemo.xlsx");
}
}
}
```
### See Also
* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
