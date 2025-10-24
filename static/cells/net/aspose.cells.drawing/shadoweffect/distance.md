##ShadowEffect.Distance
ShadowEffect property. Gets and sets the distance of the shadow. Range from 0 to 200 points
## ShadowEffect.Distance property
Gets and sets the distance of the shadow. Range from 0 to 200 points.
```csharp
public double Distance { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShadowEffectPropertyDistanceDemo
{
public static void Run()
{
// Create new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add rectangle shape
RectangleShape rectangle = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 150, 100);
// Configure shadow effect
ShadowEffect shadow = rectangle.ShadowEffect;
shadow.PresetType = PresetShadowType.OffsetDiagonalTopRight;
// Create CellsColor object and set ARGB values
CellsColor color = workbook.CreateCellsColor();
color.Argb = (128 << 24) | (255 << 16) | (0 << 8) | 0; // Semi-transparent red
shadow.Color = color;
shadow.Transparency = 0.3;
shadow.Blur = 15;
shadow.Angle = 45;
shadow.Distance = 20; // Set distance to 20 points
// Display shadow distance
Console.WriteLine("Shadow Distance: " + shadow.Distance + " points");
// Save workbook with shadow effect
workbook.Save("ShadowEffectPropertyDistanceDemo_out.xlsx");
}
}
}
```
### See Also
* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
