##Enum LightRigType
Aspose.Cells.Drawing.LightRigType enum. Represents a preset light right that can be applied to a shape
## LightRigType enumeration
Represents a preset light right that can be applied to a shape
```csharp
public enum LightRigType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Balanced | `0` | Balanced |
| BrightRoom | `1` | Bright room |
| Chilly | `2` | Chilly |
| Contrasting | `3` | Contrasting |
| Flat | `4` | Flat |
| Flood | `5` | Flood |
| Freezing | `6` | Freezing |
| Glow | `7` | Glow |
| Harsh | `8` | Harsh |
| LegacyFlat1 | `9` | LegacyFlat1 |
| LegacyFlat2 | `10` | LegacyFlat2 |
| LegacyFlat3 | `11` | LegacyFlat3 |
| LegacyFlat4 | `12` | LegacyFlat4 |
| LegacyHarsh1 | `13` | LegacyHarsh1 |
| LegacyHarsh2 | `14` | LegacyHarsh2 |
| LegacyHarsh3 | `15` | LegacyHarsh3 |
| LegacyHarsh4 | `16` | LegacyHarsh4 |
| LegacyNormal1 | `17` | LegacyNormal1 |
| LegacyNormal2 | `18` | LegacyNormal2 |
| LegacyNormal3 | `19` | LegacyNormal3 |
| LegacyNormal4 | `20` | LegacyNormal4 |
| Morning | `21` | Morning |
| Soft | `22` | Soft |
| Sunrise | `23` | Sunrise |
| Sunset | `24` | Sunset |
| ThreePoint | `25` | Three point |
| TwoPoint | `26` | Two point |
| None | `27` | No light rig. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
public class LightRigTypeDemo
{
public static void LightRigTypeExample()
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
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set the chart data range
chart.SetChartDataRange("A1:B4", true);
// Access the first series in the chart
Series series = chart.NSeries[0];
// Access the shape properties of the series
ShapePropertyCollection shapeProperties = series.ShapeProperties;
// Check if the series has 3D format data
if (shapeProperties.HasFormat3D())
{
// Access the 3D format properties
Format3D format3D = shapeProperties.Format3D;
// Set the surface lighting type to Balanced
format3D.SurfaceLightingType = LightRigType.Balanced;
// Set the lighting angle
format3D.LightingAngle = 45.0;
}
// Save the workbook
workbook.Save("LightRigTypeExample.xlsx");
workbook.Save("LightRigTypeExample.pdf");
// Output the results
Console.WriteLine("LightRigType example applied and workbook saved as 'LightRigTypeExample.xlsx'.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
