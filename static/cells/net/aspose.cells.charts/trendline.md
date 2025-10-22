##Class Trendline
Aspose.Cells.Charts.Trendline class. Represents a trendline in a chart
## Trendline class
Represents a trendline in a chart.
```csharp
public class Trendline : Line
```
## Properties
| Name | Description |
| --- | --- |
| [Backward](../../aspose.cells.charts/trendline/backward/) { get; set; } | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of periods must be greater than or equal to zero. If the chart type is column ,the number of periods must be between 0 and 0.5 |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength/) { get; set; } | Specifies the length of the arrowhead for the begin of a line.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth/) { get; set; } | Specifies the width of the arrowhead for the begin of a line.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [BeginType](../../aspose.cells.drawing/line/begintype/) { get; set; } | Specifies an arrowhead for the begin of a line.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [CapType](../../aspose.cells.drawing/line/captype/) { get; set; } | Specifies the ending caps.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [Color](../../aspose.cells.drawing/line/color/) { get; set; } | Represents the Color of the line.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype/) { get; set; } | Specifies the compound line type(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [DashType](../../aspose.cells.drawing/line/dashtype/) { get; set; } | Specifies the dash line type(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [DataLabels](../../aspose.cells.charts/trendline/datalabels/) { get; } | Represents the DataLabels object for the specified series. |
| [DisplayEquation](../../aspose.cells.charts/trendline/displayequation/) { get; set; } | Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels. |
| [DisplayRSquared](../../aspose.cells.charts/trendline/displayrsquared/) { get; set; } | Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength/) { get; set; } | Specifies the length of the arrowhead for the end of a line.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth/) { get; set; } | Specifies the width of the arrowhead for the end of a line.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [EndType](../../aspose.cells.drawing/line/endtype/) { get; set; } | Specifies an arrowhead for the end of a line.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype/) { get; set; } | Gets or sets format type.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [Forward](../../aspose.cells.charts/trendline/forward/) { get; set; } | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. The number of periods must be greater than or equal to zero. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill/) { get; } | Represents gradient fill.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [Intercept](../../aspose.cells.charts/trendline/intercept/) { get; set; } | Returns or sets the point where the trendline crosses the value axis. |
| [IsAuto](../../aspose.cells.drawing/line/isauto/) { get; set; } | Indicates whether this line style is auto assigned.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor/) { get; } | Indicates whether the color of line is automatic assigned.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [IsNameAuto](../../aspose.cells.charts/trendline/isnameauto/) { get; set; } | Returns if Microsoft Excel automatically determines the name of the trendline. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible/) { get; set; } | Represents whether the line is visible.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [JoinType](../../aspose.cells.drawing/line/jointype/) { get; set; } | Specifies the joining caps.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [LegendEntry](../../aspose.cells.charts/trendline/legendentry/) { get; } | Gets the legend entry according to this trendline |
| [Name](../../aspose.cells.charts/trendline/name/) { get; set; } | Returns the name of the trendline. |
| [Order](../../aspose.cells.charts/trendline/order/) { get; set; } | Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. The order must be between 2 and 6. |
| [Period](../../aspose.cells.charts/trendline/period/) { get; set; } | Returns or sets the period for the moving-average trendline. |
| [Style](../../aspose.cells.drawing/line/style/) { get; set; } | Represents the style of the line.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor/) { get; set; } | Gets and sets the theme color.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [Transparency](../../aspose.cells.drawing/line/transparency/) { get; set; } | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear).(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [Type](../../aspose.cells.charts/trendline/type/) { get; } | Returns the trendline type. |
| [Weight](../../aspose.cells.drawing/line/weight/) { get; set; } | Gets or sets the [`WeightType`](../../aspose.cells.drawing/weighttype/) of the line.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [WeightPt](../../aspose.cells.drawing/line/weightpt/) { get; set; } | Gets or sets the weight of the line in unit of points.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
| [WeightPx](../../aspose.cells.drawing/line/weightpx/) { get; set; } | Gets or sets the weight of the line in unit of pixels.(Inherited from [`Line`](../../aspose.cells.drawing/line/).) |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
using System.Drawing;
public class TrendlineDemo
{
public static void TrendlineExample()
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
// Adding a linear trendline
int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
// Setting the custom name of the trendline
trendline.Name = "Linear";
// Displaying the equation on chart
trendline.DisplayEquation = true;
// Displaying the R-Squared value on chart
trendline.DisplayRSquared = true;
// Setting additional properties
trendline.IsNameAuto = false;
trendline.Order = 2;
trendline.Period = 3;
trendline.Forward = 1.5;
trendline.Backward = 0.5;
trendline.Intercept = 0.0;
trendline.CompoundType = Aspose.Cells.Drawing.MsoLineStyle.ThickThin;
trendline.DashType = Aspose.Cells.Drawing.MsoLineDashStyle.Dash;
trendline.CapType = Aspose.Cells.Drawing.LineCapType.Round;
trendline.JoinType = Aspose.Cells.Drawing.LineJoinType.Bevel;
trendline.BeginType = Aspose.Cells.Drawing.MsoArrowheadStyle.Arrow;
trendline.EndType = Aspose.Cells.Drawing.MsoArrowheadStyle.Arrow;
trendline.BeginArrowLength = Aspose.Cells.Drawing.MsoArrowheadLength.Long;
trendline.EndArrowLength = Aspose.Cells.Drawing.MsoArrowheadLength.Short;
trendline.BeginArrowWidth = Aspose.Cells.Drawing.MsoArrowheadWidth.Wide;
trendline.EndArrowWidth = Aspose.Cells.Drawing.MsoArrowheadWidth.Narrow;
trendline.ThemeColor = new Aspose.Cells.ThemeColor(Aspose.Cells.ThemeColorType.Accent1, 0.5);
trendline.Color = Color.Red;
trendline.Transparency = 0.5;
trendline.Style = Aspose.Cells.Drawing.LineType.DashDot;
trendline.Weight = Aspose.Cells.Drawing.WeightType.WideLine;
trendline.WeightPt = 2.0;
trendline.WeightPx = 3.0;
trendline.FormattingType = Aspose.Cells.Charts.ChartLineFormattingType.Gradient;
trendline.IsVisible = true;
trendline.IsAuto = false;
// Saving the Excel file
workbook.Save("TrendlineExample.xlsx");
}
}
}
```
### See Also
* class [Line](../../aspose.cells.drawing/line/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
