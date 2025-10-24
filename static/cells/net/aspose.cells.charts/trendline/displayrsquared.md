##Trendline.DisplayRSquared
Trendline property. Represents if the Rsquared value of the trendline is displayed on the chart in the same data label as the equation. Setting this property to True automatically turns on data labels
## Trendline.DisplayRSquared property
Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels.
```csharp
public bool DisplayRSquared { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TrendlinePropertyDisplayRSquaredDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(1);
worksheet.Cells["A2"].PutValue(2);
worksheet.Cells["A3"].PutValue(3);
worksheet.Cells["A4"].PutValue(4);
worksheet.Cells["B1"].PutValue(2);
worksheet.Cells["B2"].PutValue(4);
worksheet.Cells["B3"].PutValue(6);
worksheet.Cells["B4"].PutValue(8);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B4", true);
// Add a trendline and get it by index
int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
trendline.Name = "Linear Trend";
// Demonstrate DisplayRSquared property
trendline.DisplayRSquared = true;
trendline.DisplayEquation = true;
// Save the workbook
workbook.Save("TrendlineDisplayRSquaredDemo.xlsx");
}
}
}
```
### See Also
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
