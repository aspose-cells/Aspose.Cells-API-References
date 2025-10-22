##Class ShapePropertyCollection
Aspose.Cells.Drawing.ShapePropertyCollection class. This class specifies the visual shape properties for a chart element or shape
## ShapePropertyCollection class
This class specifies the visual shape properties for a chart element or shape.
```csharp
public class ShapePropertyCollection
```
## Properties
| Name | Description |
| --- | --- |
| [Format3D](../../aspose.cells.drawing/shapepropertycollection/format3d/) { get; } | Represents a [`Format3D`](./format3d/) object that specifies 3D shape properties for the chart element or shape. |
| [GlowEffect](../../aspose.cells.drawing/shapepropertycollection/gloweffect/) { get; } | Represents a [`GlowEffect`](./gloweffect/) object that specifies glow effect for the chart element or shape. |
| [ShadowEffect](../../aspose.cells.drawing/shapepropertycollection/shadoweffect/) { get; } | Represents a [`ShadowEffect`](./shadoweffect/) object that specifies shadow effect for the chart element or shape. |
| [SoftEdgeRadius](../../aspose.cells.drawing/shapepropertycollection/softedgeradius/) { get; set; } | Gets and sets the radius of blur to apply to the edges, in unit of points. |
## Methods
| Name | Description |
| --- | --- |
| [ClearFormat3D](../../aspose.cells.drawing/shapepropertycollection/clearformat3d/)() | Clears the 3D shape properties of the shape. |
| [ClearGlowEffect](../../aspose.cells.drawing/shapepropertycollection/cleargloweffect/)() | Clears the glow effect of the shape. |
| [ClearShadowEffect](../../aspose.cells.drawing/shapepropertycollection/clearshadoweffect/)() | Clears the shadow effect of the chart element or shape. |
| [HasFormat3D](../../aspose.cells.drawing/shapepropertycollection/hasformat3d/)() | Indicates if the shape has 3d format data. |
| [HasGlowEffect](../../aspose.cells.drawing/shapepropertycollection/hasgloweffect/)() | Indicates if the shape has glow effect data. |
| [HasShadowEffect](../../aspose.cells.drawing/shapepropertycollection/hasshadoweffect/)() | Indicates if the shape has shadow effect data. |
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassShapePropertyCollectionDemo
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
// Set series colors
series.Area.BackgroundColor = Color.Blue;
series.Area.ForegroundColor = Color.Blue;
series.Border.Color = Color.Blue;
// Save the workbook
workbook.Save("ShapePropertyCollectionDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
