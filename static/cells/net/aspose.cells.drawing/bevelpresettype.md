##Enum BevelPresetType
Aspose.Cells.Drawing.BevelPresetType enum. Represents a preset for a type of bevel which can be applied to a shape in 3D
## BevelPresetType enumeration
Represents a preset for a type of bevel which can be applied to a shape in 3D.
```csharp
public enum BevelPresetType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No bevel |
| Angle | `1` | Angle |
| ArtDeco | `2` | Art deco |
| Circle | `3` | Circle |
| Convex | `4` | Convex |
| CoolSlant | `5` | Cool slant |
| Cross | `6` | Cross |
| Divot | `7` | Divot |
| HardEdge | `8` | Hard edge |
| RelaxedInset | `9` | Relaxed inset |
| Riblet | `10` | Riblet |
| Slope | `11` | Slope |
| SoftRound | `12` | Soft round |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System;
public class BevelPresetTypeDemo
{
public static void BevelPresetTypeExample()
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
// Access the chart's title and set its text
chart.Title.Text = "Sample Chart with Bevel";
// Access the chart's plot area
PlotArea plotArea = chart.PlotArea;
// Access the shape properties of the plot area
ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;
// Access the 3D format properties
Format3D format3D = shapeProperties.Format3D;
// Access the top bevel properties
Bevel topBevel = format3D.TopBevel;
// Set the bevel type to "Angle"
topBevel.Type = BevelPresetType.Angle;
// Set the width and height of the bevel
topBevel.Width = 10;
topBevel.Height = 10;
// Save the workbook
workbook.Save("BevelPresetTypeExample.xlsx");
workbook.Save("BevelPresetTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
