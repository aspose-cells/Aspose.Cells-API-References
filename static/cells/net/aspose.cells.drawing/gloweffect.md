##Class GlowEffect
Aspose.Cells.Drawing.GlowEffect class. This class specifies a glow effect in which a color blurred outline is added outside the edges of the object
## GlowEffect class
This class specifies a glow effect, in which a color blurred outline is added outside the edges of the object.
```csharp
public class GlowEffect
```
## Properties
| Name | Description |
| --- | --- |
| [Color](../../aspose.cells.drawing/gloweffect/color/) { get; set; } | Gets the color of the glow effect. |
| [Radius](../../aspose.cells.drawing/gloweffect/radius/) { get; set; } | (**Obsolete.**) Gets and sets the radius of the glow, in unit of points. |
| [Size](../../aspose.cells.drawing/gloweffect/size/) { get; set; } | Gets and sets the radius of the glow, in unit of points. |
| [Transparency](../../aspose.cells.drawing/gloweffect/transparency/) { get; set; } | Gets and sets the degree of transparency of the glow effect. Range from 0.0 (opaque) to 1.0 (clear). |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class GlowEffectDemo
{
public static void GlowEffectExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an arc shape to the worksheet
ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);
// Set the placement of the arc
arcShape.Placement = PlacementType.FreeFloating;
// Set the fill format
arcShape.Fill.FillType = FillType.Solid;
arcShape.Fill.SolidFill.Color = Color.Blue;
// Set the line style
arcShape.Line.CompoundType = MsoLineStyle.Single;
arcShape.Line.Weight = 2;
arcShape.Line.FillType = FillType.Solid;
arcShape.Line.SolidFill.Color = Color.Red;
arcShape.Line.DashStyle = MsoLineDashStyle.Solid;
// Create a GlowEffect instance and set its properties
GlowEffect glowEffect = arcShape.Glow;
glowEffect.Color = workbook.CreateCellsColor();
glowEffect.Color.Color = Color.Yellow;
glowEffect.Radius = 10.0;
glowEffect.Transparency = 0.5;
// Save the workbook
workbook.Save("GlowEffectExample.xlsx");
workbook.Save("GlowEffectExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
