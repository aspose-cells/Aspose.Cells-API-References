##Series.ShapeProperties
Series property. Gets the ShapePropertyCollection object that holds the visual shape properties of the Series
## Series.ShapeProperties property
Gets the [`ShapePropertyCollection`](../../../aspose.cells.drawing/shapepropertycollection/) object that holds the visual shape properties of the Series.
```csharp
public ShapePropertyCollection ShapeProperties { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class SeriesPropertyShapePropertiesDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data
chart.NSeries.Add("Sheet1!B2:B4", true);
chart.NSeries.CategoryData = "Sheet1!A2:A4";
// Get first series and its shape properties
Aspose.Cells.Charts.Series series = chart.NSeries[0];
ShapePropertyCollection shapeProperties = series.ShapeProperties;
// Configure 3D format and bevel
Format3D format3D = shapeProperties.Format3D;
Bevel topBevel = format3D.TopBevel;
topBevel.Type = BevelPresetType.Circle;
topBevel.Height = 2;
topBevel.Width = 5;
// Configure material and lighting
format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
format3D.SurfaceLightingType = LightRigType.ThreePoint;
format3D.LightingAngle = 20;
// Set series colors
series.Area.BackgroundColor = Color.Blue;
series.Area.ForegroundColor = Color.Blue;
series.Border.Color = Color.Blue;
// Save the workbook
workbook.Save("SeriesShapePropertiesDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [ShapePropertyCollection](../../../aspose.cells.drawing/shapepropertycollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
