##ShapePath.ArcTo
ShapePath method. Appends an elliptical arc to the current figure. The starting point is the end point of the current figure
## ShapePath.ArcTo method
Appends an elliptical arc to the current figure. The starting point is the end point of the current figure.
```csharp
public void ArcTo(float wR, float hR, float stAng, float swAng)
```
| Parameter | Type | Description |
| --- | --- | --- |
| wR | Single | The half-width of the rectangular area of ​​the ellipse that draws the arc(Unit: Pixel). |
| hR | Single | The half-height of the rectangular area of ​​the ellipse that draws the arc(Unit: Pixel). |
| stAng | Single | The starting angle of the arc, measured in degrees clockwise from the x-axis(Unit: Degree). This angle will specify what angle along the supposed circle path will be used as the start position for drawing the arc. This start angle will be locked to the last known pen position in the shape path. Thus guaranteeing a continuos shape path. |
| swAng | Single | The swing angle for an arc. This angle will specify how far angle-wise along the supposed cicle path the arc will be extended. The extension from the start angle will always be in the clockwise direction around the supposed circle.(Unit: Degree) |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ShapePathMethodArcToWithSingleSingleSingleSingleDemo
{
public static void Run()
{
//Create a new shape path
ShapePath shapePath = new ShapePath();
shapePath.MoveTo(60, 45);
shapePath.ArcTo(25, 25, 0, 270);
shapePath.Close();
shapePath.MoveTo(60, 20);
shapePath.LineTo(110, 70);
shapePath.LineTo(125, 155.5f);
shapePath.ArcTo(35.5f, 35.5f, 0, 270);
shapePath.Close();
shapePath.MoveTo(150, 45);
shapePath.ArcTo(25, 25, 0, 270);
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
Workbook workbook = new Workbook();
//add free form
workbook.Worksheets[0].Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath, shapePath1 });
// Save the result
workbook.Save("ShapePathMethodArcToDemo.xlsx");
}
}
}
```
### See Also
* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
