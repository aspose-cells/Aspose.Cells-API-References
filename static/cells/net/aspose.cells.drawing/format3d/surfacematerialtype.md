##Format3D.SurfaceMaterialType
Format3D property. Gets and sets the material type which is combined with the lighting properties to give the final look and feel of a shape. Default value is PresetMaterialType.WarmMatte
## Format3D.SurfaceMaterialType property
Gets and sets the material type which is combined with the lighting properties to give the final look and feel of a shape. Default value is PresetMaterialType.WarmMatte.
```csharp
public PresetMaterialType SurfaceMaterialType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class Format3DPropertySurfaceMaterialTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["A2"].PutValue("Product A");
worksheet.Cells["A3"].PutValue("Product B");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(1200);
worksheet.Cells["B3"].PutValue(1500);
// Create 3D column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B3", true);
// Configure 3D format properties
Format3D format3D = chart.NSeries[0].ShapeProperties.Format3D;
format3D.SurfaceMaterialType = PresetMaterialType.Metal;
format3D.LightingAngle = 30;
format3D.SurfaceLightingType = LightRigType.BrightRoom;
workbook.Save("Format3DPropertySurfaceMaterialTypeDemo.xlsx");
Console.WriteLine("Workbook saved with 3D chart using Metal surface material.");
}
}
}
```
### See Also
* enum [PresetMaterialType](../../presetmaterialtype/)
* class [Format3D](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
