##Format3D.SurfaceLightingType
Format3D property. Gets and sets the lighting type which is to be applied to the scene of the shape. Default value is LightRigType.ThreePoint
## Format3D.SurfaceLightingType property
Gets and sets the lighting type which is to be applied to the scene of the shape. Default value is LightRigType.ThreePoint.
```csharp
public LightRigType SurfaceLightingType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class Format3DPropertySurfaceLightingTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Data");
worksheet.Cells["A2"].PutValue(5);
worksheet.Cells["A3"].PutValue(8);
worksheet.Cells["A4"].PutValue(12);
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.SetChartDataRange("A1:A4", true);
Series series = chart.NSeries[0];
Format3D format3D = series.ShapeProperties.Format3D;
format3D.SurfaceMaterialType = PresetMaterialType.Plastic;
format3D.SurfaceLightingType = LightRigType.ThreePoint;
format3D.LightingAngle = 30;
workbook.Save("Format3DPropertySurfaceLightingTypeDemo.xlsx");
Console.WriteLine("3D chart with SurfaceLightingType set created successfully.");
}
}
}
```
### See Also
* enum [LightRigType](../../lightrigtype/)
* class [Format3D](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
