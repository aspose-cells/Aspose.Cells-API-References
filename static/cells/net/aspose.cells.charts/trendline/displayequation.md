##Trendline.DisplayEquation
Trendline property. Represents if the equation for the trendline is displayed on the chart in the same data label as the Rsquared value. Setting this property to True automatically turns on data labels
## Trendline.DisplayEquation property
Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels.
```csharp
public bool DisplayEquation { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class TrendlinePropertyDisplayEquationDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["A4"].PutValue(200);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
worksheet.Cells["B4"].PutValue(40);
// Create chart
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Add series and trendline
chart.NSeries.Add("A1:B4", true);
int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
// Configure trendline properties
trendline.DisplayEquation = true;
trendline.DisplayRSquared = false;
trendline.Color = Color.Blue;
workbook.Save("TrendlineDisplayEquationDemo.xlsx");
}
}
}
```
### See Also
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
