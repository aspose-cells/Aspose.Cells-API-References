##GlowEffect.Transparency
GlowEffect property. Gets and sets the degree of transparency of the glow effect. Range from 0.0 opaque to 1.0 clear
## GlowEffect.Transparency property
Gets and sets the degree of transparency of the glow effect. Range from 0.0 (opaque) to 1.0 (clear).
```csharp
public double Transparency { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class GlowEffectPropertyTransparencyDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
Shape shape = sheet.Shapes.AddAutoShape(AutoShapeType.RoundedRectangle, 0, 10, 0, 10, 200, 100);
shape.Glow.Size = 8;
shape.Glow.Transparency = 0.6;
CellsColor glowColor = shape.Glow.Color;
glowColor.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);
wb.Save("output/glow_transparency_demo.xlsx");
}
}
}
```
### See Also
* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
