##ShapePropertyCollection.ClearGlowEffect
ShapePropertyCollection method. Clears the glow effect of the shape
## ShapePropertyCollection.ClearGlowEffect method
Clears the glow effect of the shape.
```csharp
public void ClearGlowEffect()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class ShapePropertyCollectionMethodClearGlowEffectDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a sample chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 10);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Add sample data
worksheet.Cells["A1"].PutValue("Category 1");
worksheet.Cells["A2"].PutValue("Category 2");
worksheet.Cells["B1"].PutValue(10);
worksheet.Cells["B2"].PutValue(20);
chart.NSeries.Add("B1:B2", true);
chart.NSeries.CategoryData = "A1:A2";
// Access shape properties of the first series
Aspose.Cells.Charts.Series series = chart.NSeries[0];
ShapePropertyCollection shapeProperties = series.ShapeProperties;
// Configure 3D format and bevel
Format3D format3D = shapeProperties.Format3D;
Bevel topBevel = format3D.TopBevel;
topBevel.Type = BevelPresetType.Circle;
topBevel.Height = 2;
topBevel.Width = 5;
format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
format3D.SurfaceLightingType = LightRigType.ThreePoint;
format3D.LightingAngle = 20;
GlowEffect glowEffect = shapeProperties.GlowEffect;
glowEffect.Size = 30;
glowEffect.Color.Color = Color.Red;
// Set series colors
series.Area.BackgroundColor = Color.Blue;
series.Area.ForegroundColor = Color.Blue;
series.Border.Color = Color.Blue;
// Save the result
workbook.Save("ShapePropertyCollectionMethodClearGlowEffectDemo.xlsx");
shapeProperties.ClearGlowEffect();
workbook.Save("ShapePropertyCollectionMethodClearGlowEffectDemo2.xlsx");
}
}
}
```
### See Also
* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
