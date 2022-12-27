---
title: Trendline
second_title: Aspose.Cells for .NET API Reference
description: Represents a trendline in a chart.
type: docs
weight: 990
url: /net/aspose.cells.charts/trendline/
---
## Trendline class

Represents a trendline in a chart.

```csharp
public class Trendline : Line
```

## Properties

| Name | Description |
| --- | --- |
| [Backward](../../aspose.cells.charts/trendline/backward) { get; set; } | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of periods must be greater than and equal to zero. If the chart type is column ,the number of periods must be between 0 and 0.5 |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | Specifies the length of the arrowhead for the begin of a line. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | Specifies the width of the arrowhead for the begin of a line. |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | Specifies an arrowhead for the begin of a line. |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | Specifies the ending caps. |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | Represents the Color of the line. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | Specifies the compound line type |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | Specifies the dash line type |
| [DataLabels](../../aspose.cells.charts/trendline/datalabels) { get; } | Represents the DataLabels object for the specified ASeries. |
| [DisplayEquation](../../aspose.cells.charts/trendline/displayequation) { get; set; } | Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels. |
| [DisplayRSquared](../../aspose.cells.charts/trendline/displayrsquared) { get; set; } | Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | Specifies the length of the arrowhead for the end of a line. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | Specifies the width of the arrowhead for the end of a line. |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | Specifies an arrowhead for the end of a line. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | Gets or sets format type. |
| [Forward](../../aspose.cells.charts/trendline/forward) { get; set; } | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. The number of periods must be greater than and equal to zero. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | Represents gradient fill. |
| [Intercept](../../aspose.cells.charts/trendline/intercept) { get; set; } | Returns or sets the point where the trendline crosses the value axis. |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | Indicates whether this line style is auto assigned. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | Indicates whether the color of line is automatic assigned. |
| [IsNameAuto](../../aspose.cells.charts/trendline/isnameauto) { get; set; } | Returns if Microsoft Excel automatically determines the name of the trendline. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | Represents whether the line is visible. |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | Specifies the joining caps. |
| [LegendEntry](../../aspose.cells.charts/trendline/legendentry) { get; } | Gets the legend entry according to this trendline |
| [Name](../../aspose.cells.charts/trendline/name) { get; set; } | Returns the name of the trendline. |
| [Order](../../aspose.cells.charts/trendline/order) { get; set; } | Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. The order must be between 2 and 6. |
| [Period](../../aspose.cells.charts/trendline/period) { get; set; } | Returns or sets the period for the moving-average trendline. |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | Represents the style of the line. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | Gets and sets the theme color. |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [Type](../../aspose.cells.charts/trendline/type) { get; } | Returns the trendline type. |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | Gets or sets the [`WeightType`](../../aspose.cells.drawing/weighttype) of the line. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | Gets or sets the weight of the line in unit of points. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | Gets or sets the weight of the line in unit of pixels. |

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Adding a new worksheet to the Excel object
int sheetIndex = workbook.Worksheets.Add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.Worksheets[sheetIndex];
//Adding a sample value to "A1" cell
worksheet.Cells["A1"].PutValue(50);
//Adding a sample value to "A2" cell
worksheet.Cells["A2"].PutValue(100);
//Adding a sample value to "A3" cell
worksheet.Cells["A3"].PutValue(150);
//Adding a sample value to "A4" cell
worksheet.Cells["A4"].PutValue(200);
//Adding a sample value to "B1" cell
worksheet.Cells["B1"].PutValue(60);
//Adding a sample value to "B2" cell
worksheet.Cells["B2"].PutValue(32);
//Adding a sample value to "B3" cell
worksheet.Cells["B3"].PutValue(50);
//Adding a sample value to "B4" cell
worksheet.Cells["B4"].PutValue(40);
//Adding a sample value to "C1" cell as category data
worksheet.Cells["C1"].PutValue("Q1");
//Adding a sample value to "C2" cell as category data
worksheet.Cells["C2"].PutValue("Q2");
//Adding a sample value to "C3" cell as category data
worksheet.Cells["C3"].PutValue("Y1");
//Adding a sample value to "C4" cell as category data
worksheet.Cells["C4"].PutValue("Y2");
//Adding a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
//Accessing the instance of the newly added chart
Chart chart = worksheet.Charts[chartIndex];
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.NSeries.Add("A1:B4", true);
//Setting the data source for the category data of NSeries
chart.NSeries.CategoryData = "C1:C4";
//adding a linear trendline
int index = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
Trendline trendline = chart.NSeries[0].TrendLines[index];
//Setting the custom name of the trendline.
trendline.Name = "Linear";
//Displaying the equation on chart
trendline.DisplayEquation = true;
//Displaying the R-Squared value on chart
trendline.DisplayRSquared = true;
//Saving the Excel file
workbook.Save("book1.xls");

[Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Adding a new worksheet to the Excel object
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'Obtaining the reference of the newly added worksheet by passing its sheet index
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)
'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)
'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)
'Adding a sample value to "A4" cell
worksheet.Cells("A4").PutValue(200)
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'Adding a sample value to "B4" cell
worksheet.Cells("B4").PutValue(40)
'Adding a sample value to "C1" cell as category data
worksheet.Cells("C1").PutValue("Q1")
'Adding a sample value to "C2" cell as category data
worksheet.Cells("C2").PutValue("Q2")
'Adding a sample value to "C3" cell as category data
worksheet.Cells("C3").PutValue("Y1")
'Adding a sample value to "C4" cell as category data
worksheet.Cells("C4").PutValue("Y2")
'Adding a chart to the worksheet
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Accessing the instance of the newly added chart
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.NSeries.Add("A1:B4", True)
'Setting the data source for the category data of NSeries
Chart.NSeries.CategoryData = "C1:C4"
'adding a linear trendline
Dim index As Int32 = chart.NSeries(0).TrendLines.Add(TrendlineType.Linear)
Dim trendline As Trendline = chart.NSeries(0).TrendLines(index)
'Setting the custom name of the trendline.
trendline.Name = "Linear"
'Displaying the equation on chart
trendline.DisplayEquation = True
'Displaying the R-Squared value on chart
trendline.DisplayRSquared = True
'Saving the Excel file
workbook.Save("book1.xls")
```

### See Also

* class [Line](../../aspose.cells.drawing/line)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
