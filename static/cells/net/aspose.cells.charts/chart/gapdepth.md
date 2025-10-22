##Chart.GapDepth
Chart property. Gets or sets the distance between the data series in a 3D chart as a percentage of the marker width. The value of this property must be between 0 and 500
## Chart.GapDepth property
Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width. The value of this property must be between 0 and 500.
```csharp
public int GapDepth { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertyGapDepthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Q1");
worksheet.Cells["A3"].PutValue("Q2");
worksheet.Cells["A4"].PutValue("Q3");
worksheet.Cells["B1"].PutValue("Series 1");
worksheet.Cells["B2"].PutValue(120);
worksheet.Cells["B3"].PutValue(150);
worksheet.Cells["B4"].PutValue(180);
worksheet.Cells["C1"].PutValue("Series 2");
worksheet.Cells["C2"].PutValue(90);
worksheet.Cells["C3"].PutValue(110);
worksheet.Cells["C4"].PutValue(130);
// Add a 3D column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:C4", true);
chart.NSeries.CategoryData = "A2:A4";
// Set GapDepth property (controls the distance between data series in 3D charts)
chart.GapDepth = 150; // Value between 0-500
// Save the workbook
workbook.Save("ChartGapDepthDemo.xlsx");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
