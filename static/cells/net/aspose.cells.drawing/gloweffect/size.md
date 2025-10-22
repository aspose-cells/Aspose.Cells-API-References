##GlowEffect.Size
GlowEffect property. Gets and sets the radius of the glow in unit of points
## GlowEffect.Size property
Gets and sets the radius of the glow, in unit of points.
```csharp
public double Size { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class GlowEffectPropertySizeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RoundedRectangle, 10, 10, 200, 100, 200, 100);
// Set glow effect properties
shape.Glow.Size = 8;
shape.Glow.Transparency = 0.6;
shape.Glow.Color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
