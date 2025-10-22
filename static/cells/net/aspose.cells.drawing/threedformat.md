##Class ThreeDFormat
Aspose.Cells.Drawing.ThreeDFormat class. Represents a shapes threedimensional formatting
## ThreeDFormat class
Represents a shape's three-dimensional formatting.
```csharp
public class ThreeDFormat
```
## Properties
| Name | Description |
| --- | --- |
| [BottomBevelHeight](../../aspose.cells.drawing/threedformat/bottombevelheight/) { get; set; } | Gets and sets the height of the bottom bevel, or how far into the shape it is applied. In unit of Points. |
| [BottomBevelType](../../aspose.cells.drawing/threedformat/bottombeveltype/) { get; set; } | Gets and sets the type of the bottom bevel, or how far into the shape it is applied. In unit of Points. |
| [BottomBevelWidth](../../aspose.cells.drawing/threedformat/bottombevelwidth/) { get; set; } | Gets and sets the width of the bottom bevel, or how far into the shape it is applied. In unit of Points. |
| [ContourColor](../../aspose.cells.drawing/threedformat/contourcolor/) { get; set; } | Gets and sets the contour color on a shape. |
| [ContourWidth](../../aspose.cells.drawing/threedformat/contourwidth/) { get; set; } | Gets and sets the contour width on the shape, in unit of points. |
| [ExtrusionColor](../../aspose.cells.drawing/threedformat/extrusioncolor/) { get; set; } | Gets the extrusion color on a shape. |
| [ExtrusionHeight](../../aspose.cells.drawing/threedformat/extrusionheight/) { get; set; } | Gets and sets the extrusion height of the applied to the shape, in unit of points. |
| [LightAngle](../../aspose.cells.drawing/threedformat/lightangle/) { get; set; } | Gets and sets the angle of the extrusion lights. |
| [Lighting](../../aspose.cells.drawing/threedformat/lighting/) { get; set; } | Gets and sets type of light rig. |
| [LightingDirection](../../aspose.cells.drawing/threedformat/lightingdirection/) { get; set; } | Gets and sets the direction from which the light rig is oriented in relation to the scene. |
| [Material](../../aspose.cells.drawing/threedformat/material/) { get; set; } | Represents the preset material which is combined with the lighting properties to give the final look and feel of a shape. |
| [Perspective](../../aspose.cells.drawing/threedformat/perspective/) { get; set; } | Gets and sets the angle at which a ThreeDFormat object can be viewed. |
| [PresetCameraType](../../aspose.cells.drawing/threedformat/presetcameratype/) { get; set; } | Gets and sets the extrusion preset camera type. |
| [RotationX](../../aspose.cells.drawing/threedformat/rotationx/) { get; set; } | Gets and sets the rotation of the extruded shape around the x-axis in degrees. |
| [RotationY](../../aspose.cells.drawing/threedformat/rotationy/) { get; set; } | Gets and sets the rotation of the extruded shape around the y-axis in degrees. |
| [RotationZ](../../aspose.cells.drawing/threedformat/rotationz/) { get; set; } | Gets and sets the rotation of the extruded shape around the z-axis in degrees. |
| [TopBevelHeight](../../aspose.cells.drawing/threedformat/topbevelheight/) { get; set; } | Gets and sets the height of the top bevel, or how far into the shape it is applied. In unit of Points. |
| [TopBevelType](../../aspose.cells.drawing/threedformat/topbeveltype/) { get; set; } | Gets and sets the type of the top bevel, or how far into the shape it is applied. In unit of Points. |
| [TopBevelWidth](../../aspose.cells.drawing/threedformat/topbevelwidth/) { get; set; } | Gets and sets the width of the top bevel, or how far into the shape it is applied. In unit of Points. |
| [Z](../../aspose.cells.drawing/threedformat/z/) { get; set; } | Defines the distance from ground for the 3D shape. |
## Methods
| Name | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/threedformat/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/threedformat/gethashcode/)() | Gets hashcode. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassThreeDFormatDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 210, 210, 200, 200);
ThreeDFormat threeDFormat = shape.ThreeDFormat;
threeDFormat.TopBevelType = BevelType.SoftRound;
threeDFormat.TopBevelWidth = 10;
threeDFormat.TopBevelHeight = 10;
threeDFormat.BottomBevelType = BevelType.Divot;
threeDFormat.BottomBevelWidth = 5;
threeDFormat.BottomBevelHeight = 5;
threeDFormat.ExtrusionColor.Color = System.Drawing.Color.Blue;
threeDFormat.ExtrusionHeight = 20;
workbook.Save("ThreeDFormatDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
