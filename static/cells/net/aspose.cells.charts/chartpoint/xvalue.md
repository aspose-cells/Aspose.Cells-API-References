##ChartPoint.XValue
ChartPoint property. Gets or sets the X value of the chart point
## ChartPoint.XValue property
Gets or sets the X value of the chart point.
```csharp
public object XValue { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class ChartPointPropertyXValueDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Adding sample data
worksheet.Cells["A1"].PutValue("Category 1");
worksheet.Cells["A2"].PutValue("Category 2");
worksheet.Cells["A3"].PutValue("Category 3");
worksheet.Cells["B1"].PutValue(50);
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(150);
// Adding a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Setting chart data source
chart.NSeries.Add("B1:B3", true);
chart.NSeries.CategoryData = "A1:A3";
// Customizing data points
for (int i = 0; i < chart.NSeries[0].Points.Count; i++)
{
ChartPoint point = chart.NSeries[0].Points[i];
// Demonstrating XValue property usage
point.XValue = "Modified " + (i + 1);
// Additional formatting for visibility
point.Area.ForegroundColor = Color.FromArgb(100 + i * 50, 150, 200);
}
workbook.Save("ChartPointXValueDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
