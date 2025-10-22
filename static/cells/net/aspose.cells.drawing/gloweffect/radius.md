##GlowEffect.Radius
GlowEffect property. Gets and sets the radius of the glow in unit of points
## GlowEffect.Radius property
Gets and sets the radius of the glow, in unit of points.
```csharp
[Obsolete("Use GlowEffect.Size property instead.")]
public double Radius { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use GlowEffect.Size property. This property will be removed 6 months later since September 2016. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class GlowEffectPropertyRadiusDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);
arcShape.Placement = PlacementType.FreeFloating;
arcShape.Fill.FillType = FillType.Solid;
arcShape.Fill.SolidFill.Color = System.Drawing.Color.Blue;
GlowEffect glowEffect = arcShape.Glow;
glowEffect.Color = workbook.CreateCellsColor();
glowEffect.Color.Color = System.Drawing.Color.Yellow;
glowEffect.Radius = 15.0; // Demonstrating Radius property
glowEffect.Transparency = 0.3;
workbook.Save("GlowEffectRadiusDemo.xlsx");
}
}
}
```
### See Also
* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
