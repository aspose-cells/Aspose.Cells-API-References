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
| [CategoryType](../../aspose.cells.charts/axis/categorytype/) { get; set; } | Represents the type of the category axis. |
| [CrossAt](../../aspose.cells.charts/axis/crossat/) { get; set; } | Represents the point on the value axis where the category axis crosses it. |
| [CrossType](../../aspose.cells.charts/axis/crosstype/) { get; set; } | Represents the [`CrossType`](./crosstype/) on the specified axis where the other axis crosses. |
| [CustomDisplayUnit](../../aspose.cells.charts/axis/customdisplayunit/) { get; set; } | Specifies a custom value for the display unit. |
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
| [LogBase](../../aspose.cells.charts/axis/logbase/) { get; set; } | Represents the logarithmic base. Default value is 10. |
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
| [Title](../../aspose.cells.charts/axis/title/) { get; } | Gets the title of this axis in the chart. |

## Methods

| Name | Description |
| --- | --- |
| [GetAxisTexts](../../aspose.cells.charts/axis/getaxistexts/)() | Gets the labels of the axis after call Chart.Calculate() method. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class AxisDemo
    {
        public static void AxisExample()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            // Adding a new worksheet to the Workbook object
            int sheetIndex = workbook.Worksheets.Add();
            // Obtaining the reference of the newly added worksheet by passing its sheet index
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Adding sample values to cells
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            // Adding a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            // Accessing the instance of the newly added chart
            Chart chart = worksheet.Charts[chartIndex];
            // Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
            chart.NSeries.Add("A1:B3", true);

            // Accessing the value axis of the chart
            Axis valueAxis = chart.ValueAxis;
            // Setting properties of the value axis
            valueAxis.IsAutomaticMinValue = false;
            valueAxis.MinValue = 0;
            valueAxis.IsAutomaticMaxValue = false;
            valueAxis.MaxValue = 200;
            valueAxis.IsAutomaticMajorUnit = false;
            valueAxis.MajorUnit = 25;
            valueAxis.IsAutomaticMinorUnit = false;
            valueAxis.MinorUnit = 5;
            valueAxis.MajorTickMark = TickMarkType.Outside;
            valueAxis.MinorTickMark = TickMarkType.Inside;
            valueAxis.TickLabelPosition = TickLabelPositionType.NextToAxis;
            valueAxis.CrossAt = 0;
            valueAxis.CrossType = CrossType.Minimum;
            valueAxis.IsLogarithmic = false;
            valueAxis.IsPlotOrderReversed = false;
            valueAxis.AxisBetweenCategories = true;
            valueAxis.TickLabelSpacing = 1;
            valueAxis.IsAutoTickLabelSpacing = true;
            valueAxis.TickMarkSpacing = 1;
            valueAxis.DisplayUnit = DisplayUnitType.None;
            valueAxis.IsDisplayUnitLabelShown = false;
            valueAxis.CategoryType = CategoryType.AutomaticScale;
            valueAxis.BaseUnitScale = TimeUnit.Months;
            valueAxis.MajorUnitScale = TimeUnit.Months;
            valueAxis.MinorUnitScale = TimeUnit.Months;
            valueAxis.IsVisible = true;
            valueAxis.HasMultiLevelLabels = false;

            // Accessing the category axis of the chart
            Axis categoryAxis = chart.CategoryAxis;
            // Setting properties of the category axis
            categoryAxis.IsAutomaticMinValue = false;
            categoryAxis.MinValue = 0;
            categoryAxis.IsAutomaticMaxValue = false;
            categoryAxis.MaxValue = 3;
            categoryAxis.IsAutomaticMajorUnit = false;
            categoryAxis.MajorUnit = 1;
            categoryAxis.IsAutomaticMinorUnit = false;
            categoryAxis.MinorUnit = 0.5;
            categoryAxis.MajorTickMark = TickMarkType.Outside;
            categoryAxis.MinorTickMark = TickMarkType.Inside;
            categoryAxis.TickLabelPosition = TickLabelPositionType.NextToAxis;
            categoryAxis.CrossAt = 0;
            categoryAxis.CrossType = CrossType.Minimum;
            categoryAxis.IsLogarithmic = false;
            categoryAxis.IsPlotOrderReversed = false;
            categoryAxis.AxisBetweenCategories = true;
            categoryAxis.TickLabelSpacing = 1;
            categoryAxis.IsAutoTickLabelSpacing = true;
            categoryAxis.TickMarkSpacing = 1;
            categoryAxis.DisplayUnit = DisplayUnitType.None;
            categoryAxis.IsDisplayUnitLabelShown = false;
            categoryAxis.CategoryType = CategoryType.AutomaticScale;
            categoryAxis.BaseUnitScale = TimeUnit.Months;
            categoryAxis.MajorUnitScale = TimeUnit.Months;
            categoryAxis.MinorUnitScale = TimeUnit.Months;
            categoryAxis.IsVisible = true;
            categoryAxis.HasMultiLevelLabels = false;

            // Saving the Excel file
            workbook.Save("AxisExample.xlsx");
            workbook.Save("AxisExample.pdf");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


