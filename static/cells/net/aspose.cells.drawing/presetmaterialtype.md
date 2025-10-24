##Enum PresetMaterialType
Aspose.Cells.Drawing.PresetMaterialType enum. Describes surface appearance of a shape
## PresetMaterialType enumeration
Describes surface appearance of a shape.
```csharp
public enum PresetMaterialType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Clear | `0` | Clear |
| DarkEdge | `1` | Dark edge |
| Flat | `2` | Flat |
| LegacyMatte | `3` | Legacy matte |
| LegacyMetal | `4` | Legacy metal |
| LegacyPlastic | `5` | Legacy plastic |
| LegacyWireframe | `6` | Legacy wireframe |
| Matte | `7` | Matte |
| Metal | `8` | Metal |
| Plastic | `9` | Plastic |
| Powder | `10` | Powder |
| SoftEdge | `11` | Soft edge |
| SoftMetal | `12` | Soft metal |
| TranslucentPowder | `13` | Translucent powder |
| WarmMatte | `14` | Warm matte |
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
namespace AsposeCellsExamples
{
public class PresetMaterialTypeDemo
{
public static void PresetMaterialTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set the chart data range
chart.SetChartDataRange("A1:B4", true);
// Access the first series in the chart
Series series = chart.NSeries[0];
// Access the 3D format of the series
Format3D format3D = series.ShapeProperties.Format3D;
// Set the surface material type
format3D.SurfaceMaterialType = PresetMaterialType.Metal;
// Set other 3D properties
format3D.LightingAngle = 45;
format3D.SurfaceLightingType = LightRigType.ThreePoint;
// Save the workbook
workbook.Save("PresetMaterialTypeExample.xlsx");
// Output the results
Console.WriteLine("Chart with 3D format and PresetMaterialType applied has been created.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
