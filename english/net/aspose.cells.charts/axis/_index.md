---
title: Axis
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 350
url: /net/aspose.cells.charts/axis/
---
## Axis class

Encapsulates the object that represents a chart's axis.

```csharp
public class Axis
```

## Properties

| Name | Description |
| --- | --- |
| [Area](area) { get; } | Gets the [`Area`](./area). |
| [AxisBetweenCategories](axisbetweencategories) { get; set; } | Represents if the value axis crosses the category axis between categories. |
| [AxisLabels](axislabels) { get; } | Gets the labels of the axis after call Chart.Calculate() method. |
| [AxisLine](axisline) { get; } | Gets the appearance of an Axis. |
| [BaseUnitScale](baseunitscale) { get; set; } | Represents the base unit scale for the category axis. |
| [Bins](bins) { get; } | Represents bins on a chart(Histogram/Pareto) axis |
| [CategoryType](categorytype) { get; set; } | Represents the category axis type. |
| [CrossAt](crossat) { get; set; } | Represents the point on the value axis where the category axis crosses it. |
| [CrossType](crosstype) { get; set; } | Represents the [`CrossType`](./crosstype) on the specified axis where the other axis crosses. |
| [CustUnit](custunit) { get; set; } | Specifies a custom value for the display unit. |
| [DisplayUnit](displayunit) { get; set; } | Represents the unit label for the specified axis. |
| [DisplayUnitLabel](displayunitlabel) { get; } | Represents a unit label on an axis in the specified chart. Unit labels are useful for charting large values— for example, in the millions or billions. |
| [HasMultiLevelLabels](hasmultilevellabels) { get; set; } | Indicates whether the labels shall be shown as multi level. |
| [IsAutomaticMajorUnit](isautomaticmajorunit) { get; set; } | Indicates whether the major unit of the axis is automatically assigned. |
| [IsAutomaticMaxValue](isautomaticmaxvalue) { get; set; } | Indicates whether the max value is automatically assigned. |
| [IsAutomaticMinorUnit](isautomaticminorunit) { get; set; } | Indicates whether the minor unit of the axis is automatically assigned. |
| [IsAutomaticMinValue](isautomaticminvalue) { get; set; } | Indicates whether the min value is automatically assigned. |
| [IsAutoTickLabelSpacing](isautoticklabelspacing) { get; set; } | Indicates whether the spacing of tick label is automatic |
| [IsDisplayUnitLabelShown](isdisplayunitlabelshown) { get; set; } | Represents if the display unit label is shown on the specified axis. |
| [IsLogarithmic](islogarithmic) { get; set; } | Represents if the value axis scale type is logarithmic or not. |
| [IsPlotOrderReversed](isplotorderreversed) { get; set; } | Represents if Microsoft Excel plots data points from last to first. |
| [IsVisible](isvisible) { get; set; } | Represents if the axis is visible. |
| [LogBase](logbase) { get; set; } | Represents the logarithmic base. Default value is 10.Only applies for Excel2007. |
| [MajorGridLines](majorgridlines) { get; } | Represents major gridlines on a chart axis. |
| [MajorTickMark](majortickmark) { get; set; } | Represents the type of major tick mark for the specified axis. |
| [MajorUnit](majorunit) { get; set; } | Represents the major units for the axis. |
| [MajorUnitScale](majorunitscale) { get; set; } | Represents the major unit scale for the category axis. |
| [MaxValue](maxvalue) { get; set; } | Represents the maximum value on the value axis. |
| [MinorGridLines](minorgridlines) { get; } | Represents minor gridlines on a chart axis. |
| [MinorTickMark](minortickmark) { get; set; } | Represents the type of minor tick mark for the specified axis. |
| [MinorUnit](minorunit) { get; set; } | Represents the minor units for the axis. |
| [MinorUnitScale](minorunitscale) { get; set; } | Represents the major unit scale for the category axis. |
| [MinValue](minvalue) { get; set; } | Represents the minimum value on the value axis. |
| [TickLabelPosition](ticklabelposition) { get; set; } | Represents the position of tick-mark labels on the specified axis. |
| [TickLabels](ticklabels) { get; } | Returns a [`TickLabels`](./ticklabels) object that represents the tick-mark labels for the specified axis. |
| [TickLabelSpacing](ticklabelspacing) { get; set; } | Represents the number of categories or series between tick-mark labels. Applies only to category and series axes. |
| [TickMarkSpacing](tickmarkspacing) { get; set; } | Returns or sets the number of categories or series between tick marks. Applies only to category and series axes. |
| [Title](title) { get; } | Gets the axis' title. |

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

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
