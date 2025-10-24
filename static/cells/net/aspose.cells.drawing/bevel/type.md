##Bevel.Type
Bevel property. Gets and sets the preset bevel type
## Bevel.Type property
Gets and sets the preset bevel type.
```csharp
public BevelPresetType Type { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class BevelPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
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
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 10);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get the first series
Aspose.Cells.Charts.Series series = chart.NSeries[0];
// Set series color
series.Area.ForegroundColor = Color.Blue;
// Configure 3D format and bevel properties
Format3D format3D = series.ShapeProperties.Format3D;
Bevel topBevel = format3D.TopBevel;
// Demonstrate Type property usage
topBevel.Type = BevelPresetType.Circle;
topBevel.Width = 5;
topBevel.Height = 2;
// Save the workbook
workbook.Save("BevelPropertyTypeDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* enum [BevelPresetType](../../bevelpresettype/)
* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
