##Format3D.LightingAngle
Format3D property. Gets and sets the lighting angle. Range from 0 to 359.9 degrees
## Format3D.LightingAngle property
Gets and sets the lighting angle. Range from 0 to 359.9 degrees.
```csharp
public double LightingAngle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class Format3DPropertyLightingAngleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
Series series = chart.NSeries[0];
Format3D format3D = series.ShapeProperties.Format3D;
format3D.SurfaceMaterialType = PresetMaterialType.Metal;
format3D.LightingAngle = 45;
format3D.SurfaceLightingType = LightRigType.ThreePoint;
workbook.Save("Format3DLightingAngleDemo.xlsx");
Console.WriteLine("Workbook saved with 3D lighting angle set to 45 degrees.");
}
}
}
```
### See Also
* class [Format3D](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
