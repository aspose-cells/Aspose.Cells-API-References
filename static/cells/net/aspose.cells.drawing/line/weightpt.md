##Line.WeightPt
Line property. Gets or sets the weight of the line in unit of points
## Line.WeightPt property
Gets or sets the weight of the line in unit of points.
```csharp
public double WeightPt { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class LinePropertyWeightPtDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Pie, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Configure data labels
Aspose.Cells.Charts.Series series = chart.NSeries[0];
series.DataLabels.ShowValue = true;
series.HasLeaderLines = true;
// Customize leader lines
series.LeaderLines.IsAuto = false;
series.LeaderLines.Style = Aspose.Cells.Drawing.LineType.Dot;
series.LeaderLines.WeightPt = 0.25; // Demonstrate WeightPt property
series.LeaderLines.Color = Color.LightCyan;
// Save the workbook
workbook.Save("LeaderLinesDemo.xlsx");
}
}
}
```
### See Also
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
