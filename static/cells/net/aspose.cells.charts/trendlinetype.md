##Enum TrendlineType
Aspose.Cells.Charts.TrendlineType enum. Represents the trendline type
## TrendlineType enumeration
Represents the trendline type.
```csharp
public enum TrendlineType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Exponential | `0` | Exponential |
| Linear | `1` | Linear |
| Logarithmic | `2` | Logarithmic |
| MovingAverage | `3` | MovingAverage |
| Polynomial | `4` | Polynomial |
| Power | `5` | Power |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
using System.Drawing;
public class TrendlineTypeDemo
{
public static void TrendlineTypeExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Adding a new worksheet to the Excel object
int sheetIndex = workbook.Worksheets.Add();
// Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.Worksheets[sheetIndex];
// Adding sample values to cells
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["A4"].PutValue(200);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
worksheet.Cells["B4"].PutValue(40);
worksheet.Cells["C1"].PutValue("Q1");
worksheet.Cells["C2"].PutValue("Q2");
worksheet.Cells["C3"].PutValue("Y1");
worksheet.Cells["C4"].PutValue("Y2");
// Adding a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
// Accessing the instance of the newly added chart
Chart chart = worksheet.Charts[chartIndex];
// Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.NSeries.Add("A1:B4", true);
// Setting the data source for the category data of NSeries
chart.NSeries.CategoryData = "C1:C4";
// Adding different types of trendlines to the chart
AddTrendline(chart, 0, TrendlineType.Linear, "Linear Trendline");
AddTrendline(chart, 0, TrendlineType.Exponential, "Exponential Trendline");
AddTrendline(chart, 0, TrendlineType.Logarithmic, "Logarithmic Trendline");
AddTrendline(chart, 0, TrendlineType.MovingAverage, "Moving Average Trendline");
AddTrendline(chart, 0, TrendlineType.Polynomial, "Polynomial Trendline");
AddTrendline(chart, 0, TrendlineType.Power, "Power Trendline");
// Saving the Excel file
workbook.Save("TrendlineTypeExample.xlsx");
}
private static void AddTrendline(Chart chart, int seriesIndex, TrendlineType trendlineType, string trendlineName)
{
// Adding a trendline of the specified type to the specified series
int index = chart.NSeries[seriesIndex].TrendLines.Add(trendlineType);
Trendline trendline = chart.NSeries[seriesIndex].TrendLines[index];
// Setting the custom name of the trendline
trendline.Name = trendlineName;
// Displaying the equation on the chart
trendline.DisplayEquation = true;
// Displaying the R-Squared value on the chart
trendline.DisplayRSquared = true;
// Setting the color of the trendline
trendline.Color = Color.Red;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
