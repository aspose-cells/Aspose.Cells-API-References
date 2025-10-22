##ShapePropertyCollection.HasShadowEffect
ShapePropertyCollection method. Indicates if the shape has shadow effect data
## ShapePropertyCollection.HasShadowEffect method
Indicates if the shape has shadow effect data.
```csharp
public bool HasShadowEffect()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class ShapePropertyCollectionMethodHasShadowEffectDemo
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
ShadowEffect shadowEffect = shapeProperties.ShadowEffect;
shadowEffect.Size = 1.5;
shadowEffect.Color.Color = Color.Red;
shadowEffect.Angle = 180;
// Set series colors
series.Area.BackgroundColor = Color.Blue;
series.Area.ForegroundColor = Color.Blue;
series.Border.Color = Color.Blue;
Console.WriteLine($"Shape has shadow effect after: {shapeProperties.HasShadowEffect()}");
// Save the result
workbook.Save("ShapePropertyCollectionMethodHasShadowEffectDemo.xlsx");
}
}
}
```
### See Also
* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
