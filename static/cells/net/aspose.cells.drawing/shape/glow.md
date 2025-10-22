##Shape.Glow
Shape property. Represents a GlowEffect object that specifies glow effect for the chart element or shape
## Shape.Glow property
Represents a [`GlowEffect`](../../gloweffect/) object that specifies glow effect for the chart element or shape.
```csharp
public GlowEffect Glow { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyGlowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
// Access the glow effect
GlowEffect glow = shape.Glow;
// Set glow properties
CellsColor color = workbook.CreateCellsColor();
color.Color = System.Drawing.Color.Purple;
glow.Color = color;
glow.Size = 10; // 10 point radius
glow.Transparency = 0.5; // 50% transparency
// Save the workbook
workbook.Save("ShapeGlowDemo.xlsx");
}
}
}
```
### See Also
* class [GlowEffect](../../gloweffect/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
