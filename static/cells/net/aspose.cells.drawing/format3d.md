##Class Format3D
Aspose.Cells.Drawing.Format3D class. This class specifies the 3D shape properties for a chart element or shape
## Format3D class
This class specifies the 3D shape properties for a chart element or shape.
```csharp
public class Format3D
```
## Properties
| Name | Description |
| --- | --- |
| [LightingAngle](../../aspose.cells.drawing/format3d/lightingangle/) { get; set; } | Gets and sets the lighting angle. Range from 0 to 359.9 degrees. |
| [SurfaceLightingType](../../aspose.cells.drawing/format3d/surfacelightingtype/) { get; set; } | Gets and sets the lighting type which is to be applied to the scene of the shape. Default value is LightRigType.ThreePoint. |
| [SurfaceMaterialType](../../aspose.cells.drawing/format3d/surfacematerialtype/) { get; set; } | Gets and sets the material type which is combined with the lighting properties to give the final look and feel of a shape. Default value is PresetMaterialType.WarmMatte. |
| [TopBevel](../../aspose.cells.drawing/format3d/topbevel/) { get; } | Gets the [`Bevel`](../bevel/) object that holds the properties associated with defining a bevel on the top or front face of a shape. |
## Methods
| Name | Description |
| --- | --- |
| [HasTopBevelData](../../aspose.cells.drawing/format3d/hastopbeveldata/)() | Indicates if the shape has top bevel data. |
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
namespace AsposeCellsExamples
{
public class Format3DDemo
{
public static void RunDemo()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add some sample data
sheet.Cells["A1"].PutValue(10);
sheet.Cells["A2"].PutValue(20);
sheet.Cells["A3"].PutValue(30);
sheet.Cells["A4"].PutValue(40);
// Add a chart to the worksheet
int chartIndex = sheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 20, 10);
Chart chart = sheet.Charts[chartIndex];
// Add series to the chart
chart.NSeries.Add("A1:A4", true);
// Access the first series
Series series = chart.NSeries[0];
// Access the 3D format of the series
Format3D format3D = series.ShapeProperties.Format3D;
// Set the 3D format properties
format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
format3D.SurfaceLightingType = LightRigType.ThreePoint;
format3D.LightingAngle = 45.0;
// Check if the shape has top bevel data
if (format3D.HasTopBevelData())
{
Bevel topBevel = format3D.TopBevel;
Console.WriteLine("Top Bevel Width: " + topBevel.Width);
Console.WriteLine("Top Bevel Height: " + topBevel.Height);
}
// Save the workbook
workbook.Save("Format3DDemo.xlsx");
workbook.Save("Format3DDemo.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
