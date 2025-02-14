---
title: Class Axis
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Charts.Axis class. Encapsulates the object that represents an axis of chart
type: docs
url: /net/aspose.cells.charts/axis/
---
## Axis class

Encapsulates the object that represents an axis of chart.

```csharp
public class Axis
```

## Properties

| Name | Description |
| --- | --- |
| [Area](../../aspose.cells.charts/axis/area/) { get; } | Gets the [`Area`](./area/). |
| [AxisBetweenCategories](../../aspose.cells.charts/axis/axisbetweencategories/) { get; set; } | Represents if the value axis crosses the category axis between categories. |
| [AxisLabels](../../aspose.cells.charts/axis/axislabels/) { get; } | (**Obsolete.**) Gets the labels of the axis after call Chart.Calculate() method. |
| [AxisLine](../../aspose.cells.charts/axis/axisline/) { get; } | Gets the appearance of an Axis. |
| [BaseUnitScale](../../aspose.cells.charts/axis/baseunitscale/) { get; set; } | Represents the base unit scale for the category axis. |
| [Bins](../../aspose.cells.charts/axis/bins/) { get; } | Represents bins on a chart(Histogram/Pareto) axis |
| [CategoryType](../../aspose.cells.charts/axis/categorytype/) { get; set; } | Represents the category axis type. |
| [CoustomDisplayUnit](../../aspose.cells.charts/axis/coustomdisplayunit/) { get; set; } | Specifies a custom value for the display unit. |
| [CrossAt](../../aspose.cells.charts/axis/crossat/) { get; set; } | Represents the point on the value axis where the category axis crosses it. |
| [CrossType](../../aspose.cells.charts/axis/crosstype/) { get; set; } | Represents the [`CrossType`](./crosstype/) on the specified axis where the other axis crosses. |
| [CustomUnit](../../aspose.cells.charts/axis/customunit/) { get; set; } | (**Obsolete.**) Specifies a custom value for the display unit. |
| [CustUnit](../../aspose.cells.charts/axis/custunit/) { get; set; } | (**Obsolete.**) Specifies a custom value for the display unit. |
| [DisplayUnit](../../aspose.cells.charts/axis/displayunit/) { get; set; } | Represents the unit label for the specified axis. |
| [DisplayUnitLabel](../../aspose.cells.charts/axis/displayunitlabel/) { get; } | Represents a unit label on an axis in the specified chart. Unit labels are useful for charting large values— for example, in the millions or billions. |
| [HasMultiLevelLabels](../../aspose.cells.charts/axis/hasmultilevellabels/) { get; set; } | Indicates whether the labels shall be shown as multi level. |
| [IsAutomaticMajorUnit](../../aspose.cells.charts/axis/isautomaticmajorunit/) { get; set; } | Indicates whether the major unit of the axis is automatically assigned. |
| [IsAutomaticMaxValue](../../aspose.cells.charts/axis/isautomaticmaxvalue/) { get; set; } | Indicates whether the max value is automatically assigned. |
| [IsAutomaticMinorUnit](../../aspose.cells.charts/axis/isautomaticminorunit/) { get; set; } | Indicates whether the minor unit of the axis is automatically assigned. |
| [IsAutomaticMinValue](../../aspose.cells.charts/axis/isautomaticminvalue/) { get; set; } | Indicates whether the min value is automatically assigned. |
| [IsAutoTickLabelSpacing](../../aspose.cells.charts/axis/isautoticklabelspacing/) { get; set; } | Indicates whether the spacing of tick label is automatic |
| [IsDisplayUnitLabelShown](../../aspose.cells.charts/axis/isdisplayunitlabelshown/) { get; set; } | Represents if the display unit label is shown on the specified axis. |
| [IsLogarithmic](../../aspose.cells.charts/axis/islogarithmic/) { get; set; } | Represents if the value axis scale type is logarithmic or not. |
| [IsPlotOrderReversed](../../aspose.cells.charts/axis/isplotorderreversed/) { get; set; } | Represents if Microsoft Excel plots data points from last to first. |
| [IsVisible](../../aspose.cells.charts/axis/isvisible/) { get; set; } | Represents if the axis is visible. |
| [LogBase](../../aspose.cells.charts/axis/logbase/) { get; set; } | Represents the logarithmic base. Default value is 10.Only applies for Excel2007. |
| [MajorGridLines](../../aspose.cells.charts/axis/majorgridlines/) { get; } | Represents major gridlines on a chart axis. |
| [MajorTickMark](../../aspose.cells.charts/axis/majortickmark/) { get; set; } | Represents the type of major tick mark for the specified axis. |
| [MajorUnit](../../aspose.cells.charts/axis/majorunit/) { get; set; } | Represents the major units for the axis. |
| [MajorUnitScale](../../aspose.cells.charts/axis/majorunitscale/) { get; set; } | Represents the major unit scale for the category axis. |
| [MaxValue](../../aspose.cells.charts/axis/maxvalue/) { get; set; } | Represents the maximum value on the value axis. |
| [MinorGridLines](../../aspose.cells.charts/axis/minorgridlines/) { get; } | Represents minor gridlines on a chart axis. |
| [MinorTickMark](../../aspose.cells.charts/axis/minortickmark/) { get; set; } | Represents the type of minor tick mark for the specified axis. |
| [MinorUnit](../../aspose.cells.charts/axis/minorunit/) { get; set; } | Represents the minor units for the axis. |
| [MinorUnitScale](../../aspose.cells.charts/axis/minorunitscale/) { get; set; } | Represents the major unit scale for the category axis. |
| [MinValue](../../aspose.cells.charts/axis/minvalue/) { get; set; } | Represents the minimum value on the value axis. |
| [TickLabelPosition](../../aspose.cells.charts/axis/ticklabelposition/) { get; set; } | Represents the position of tick-mark labels on the specified axis. |
| [TickLabels](../../aspose.cells.charts/axis/ticklabels/) { get; } | Returns a [`TickLabels`](./ticklabels/) object that represents the tick-mark labels for the specified axis. |
| [TickLabelSpacing](../../aspose.cells.charts/axis/ticklabelspacing/) { get; set; } | Represents the number of categories or series between tick-mark labels. Applies only to category and series axes. |
| [TickMarkSpacing](../../aspose.cells.charts/axis/tickmarkspacing/) { get; set; } | Returns or sets the number of categories or series between tick marks. Applies only to category and series axes. |
| [Title](../../aspose.cells.charts/axis/title/) { get; } | Gets the axis' title. |

## Methods

| Name | Description |
| --- | --- |
| [GetAxisTexts](../../aspose.cells.charts/axis/getaxistexts/)() | Gets the labels of the axis after call Chart.Calculate() method. |

### Examples

From the following codes , you can learn how to set unit, maximum and minimum value of Axis.

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
//Adding a sample value to "B1" cell
worksheet.Cells["B1"].PutValue(4);
//Adding a sample value to "B2" cell
worksheet.Cells["B2"].PutValue(20);
//Adding a sample value to "B3" cell
worksheet.Cells["B3"].PutValue(50);
//Adding a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
//Accessing the instance of the newly added chart
Chart chart = worksheet.Charts[chartIndex];
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", true);
//Set the max value of value axis
chart.ValueAxis.MaxValue = 200;
//Set the min value of value axis
chart.ValueAxis.MinValue = 0;
//Set the major unit
chart.ValueAxis.MajorUnit = 25;
//Category(X) axis crosses at the maxinum value.
chart.ValueAxis.CrossType = CrossType.Maximum;
//Set he number of categories or series between tick-mark labels. 
chart.CategoryAxis.TickLabelSpacing = 2;

//do your business

//Saving the Excel file
workbook.Save("book1.xlsx");

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
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(4)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(20)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'Adding a chart to the worksheet
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5)
'Accessing the instance of the newly added chart
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", True)
'Set the max value of value axis
chart.ValueAxis.MaxValue = 200
'Set the min value of value axis
chart.ValueAxis.MinValue = 0
'Set the major unit
chart.ValueAxis.MajorUnit = 25
'Category(X) axis crosses at the maxinum value.
chart.ValueAxis.CrossType = CrossType.Maximum
'Set he number of categories or series between tick-mark labels. 
chart.CategoryAxis.TickLabelSpacing = 2
'Saving the Excel file
workbook.Save("book1.xlsx")
```

### See Also

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


