##Class Bevel
Aspose.Cells.Drawing.Bevel class. Represents a bevel of a shape
## Bevel class
Represents a bevel of a shape
```csharp
public class Bevel
```
## Properties
| Name | Description |
| --- | --- |
| [Height](../../aspose.cells.drawing/bevel/height/) { get; set; } | Gets and sets the height of the bevel, or how far above the shape it is applied. In unit of Points. |
| [Type](../../aspose.cells.drawing/bevel/type/) { get; set; } | Gets and sets the preset bevel type. |
| [Width](../../aspose.cells.drawing/bevel/width/) { get; set; } | Gets and sets the width of the bevel, or how far into the shape it is applied. In unit of Points. |
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
namespace AsposeCellsExamples
{
public class BevelDemo
{
public static void RunDemo()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
workbook.CalculateFormula();
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add data series to the chart
chart.NSeries.Add("A1:B4", true);
// Access the chart's plot area
ChartFrame plotArea = chart.PlotArea;
// Access the shape properties of the plot area
ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;
// Access the 3D format properties
Format3D format3D = shapeProperties.Format3D;
// Access the top bevel properties
Bevel topBevel = format3D.TopBevel;
// Set the width, height, and type of the bevel
topBevel.Width = 10.0;
topBevel.Height = 5.0;
topBevel.Type = BevelPresetType.Circle;
// Set other 3D format properties
format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
format3D.SurfaceLightingType = LightRigType.ThreePoint;
format3D.LightingAngle = 45.0;
// Save the workbook
workbook.Save("BevelDemo.xlsx");
workbook.Save("BevelDemo.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
