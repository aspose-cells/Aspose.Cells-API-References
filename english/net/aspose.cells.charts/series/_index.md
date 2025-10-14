---
title: Class Series
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Charts.Series class. Encapsulates the object that represents a single data series in a chart
type: docs
url: /net/aspose.cells.charts/series/
---
## Series class

Encapsulates the object that represents a single data series in a chart.

```csharp
public class Series
```

## Properties

| Name | Description |
| --- | --- |
| [Area](../../aspose.cells.charts/series/area/) { get; } | Represents the background area of Series object. |
| [Bar3DShapeType](../../aspose.cells.charts/series/bar3dshapetype/) { get; set; } | Gets or sets the 3D shape type used with the 3-D bar or column chart. |
| [Border](../../aspose.cells.charts/series/border/) { get; } | Represents border of Series object. |
| [BubbleScale](../../aspose.cells.charts/series/bubblescale/) { get; set; } | Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, corresponding to a percentage of the default size. Applies only to bubble charts. |
| [BubbleSizes](../../aspose.cells.charts/series/bubblesizes/) { get; set; } | Gets or sets the bubble sizes values of the chart series. |
| [CachedCategoryValues](../../aspose.cells.charts/series/cachedcategoryvalues/) { get; } | (**Obsolete.**) Gets the cached category values for the series |
| [CachedValues](../../aspose.cells.charts/series/cachedvalues/) { get; } | (**Obsolete.**) Gets the cached values for the series |
| [CountOfDataValues](../../aspose.cells.charts/series/countofdatavalues/) { get; } | Gets the number of the data values. |
| [DataLabels](../../aspose.cells.charts/series/datalabels/) { get; } | Represents the DataLabels object for the specified ASeries. |
| [DisplayName](../../aspose.cells.charts/series/displayname/) { get; } | Gets the series's name that displays on the chart graph. |
| [DoughnutHoleSize](../../aspose.cells.charts/series/doughnutholesize/) { get; set; } | Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart size, between 10 and 90 percent. |
| [DownBars](../../aspose.cells.charts/series/downbars/) { get; } | Returns a [`DropBars`](../dropbars/) object that represents the down bars on a line chart. Applies only to line charts. |
| [DropLines](../../aspose.cells.charts/series/droplines/) { get; } | Returns a [`Line`](../../aspose.cells.drawing/line/) object that represents the drop lines for a series on the line chart or area chart. Applies only to line chart or area charts. |
| [Explosion](../../aspose.cells.charts/series/explosion/) { get; set; } | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [FirstSliceAngle](../../aspose.cells.charts/series/firstsliceangle/) { get; set; } | Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360. |
| [GapWidth](../../aspose.cells.charts/series/gapwidth/) { get; set; } | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500. |
| [Has3DEffect](../../aspose.cells.charts/series/has3deffect/) { get; set; } | True if the series has a three-dimensional appearance. Applies only to bubble charts. |
| [HasDropLines](../../aspose.cells.charts/series/hasdroplines/) { get; set; } | True if the chart has drop lines. Applies only to line chart or area charts. |
| [HasHiLoLines](../../aspose.cells.charts/series/hashilolines/) { get; set; } | True if the line chart has high-low lines. Applies only to line charts. |
| [HasLeaderLines](../../aspose.cells.charts/series/hasleaderlines/) { get; set; } | True if the series has leader lines. |
| [HasRadarAxisLabels](../../aspose.cells.charts/series/hasradaraxislabels/) { get; set; } | True if a radar chart has category axis labels. Applies only to radar charts. |
| [HasSeriesLines](../../aspose.cells.charts/series/hasserieslines/) { get; set; } | True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts. |
| [HasUpDownBars](../../aspose.cells.charts/series/hasupdownbars/) { get; set; } | True if a line chart has up and down bars. Applies only to line charts. |
| [HiLoLines](../../aspose.cells.charts/series/hilolines/) { get; } | Returns a HiLoLines object that represents the high-low lines for a series on a line chart. Applies only to line charts. |
| [IsAutoSplit](../../aspose.cells.charts/series/isautosplit/) { get; } | Indicates whether the threshold value is automatic. |
| [IsColorVaried](../../aspose.cells.charts/series/iscolorvaried/) { get; set; } | Represents if the color of points is varied. The chart must contain only one series. |
| [IsFiltered](../../aspose.cells.charts/series/isfiltered/) { get; set; } | Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart. |
| [IsVerticalValues](../../aspose.cells.charts/series/isverticalvalues/) { get; } | Indicates whether the data source is vertical. |
| [LayoutProperties](../../aspose.cells.charts/series/layoutproperties/) { get; } | Represents the properties of layout. |
| [LeaderLines](../../aspose.cells.charts/series/leaderlines/) { get; } | Represents leader lines on a chart. Leader lines connect data labels to data points. This object isn’t a collection; there’s no object that represents a single leader line. |
| [LegendEntry](../../aspose.cells.charts/series/legendentry/) { get; } | Gets the legend entry according to this series. |
| [Marker](../../aspose.cells.charts/series/marker/) { get; } | Gets the [`marker`](./marker/). |
| [Name](../../aspose.cells.charts/series/name/) { get; set; } | Gets or sets the name of the data series. |
| [Overlap](../../aspose.cells.charts/series/overlap/) { get; set; } | Specifies how bars and columns are positioned. Can be a value between – 100 and 100. Applies only to 2-D bar and 2-D column charts. |
| [PlotOnSecondAxis](../../aspose.cells.charts/series/plotonsecondaxis/) { get; set; } | Indicates if this series is plotted on second value axis. |
| [Points](../../aspose.cells.charts/series/points/) { get; } | Gets the collection of points in a series in a chart. |
| [SecondPlotSize](../../aspose.cells.charts/series/secondplotsize/) { get; set; } | Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of the size of the primary pie. Can be a value from 5 to 200. |
| [SeriesLines](../../aspose.cells.charts/series/serieslines/) { get; } | Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. Applies only to stacked bar and stacked column charts. |
| [Shadow](../../aspose.cells.charts/series/shadow/) { get; set; } | True if the series has a shadow. |
| [ShapeProperties](../../aspose.cells.charts/series/shapeproperties/) { get; } | Gets the [`ShapePropertyCollection`](../../aspose.cells.drawing/shapepropertycollection/) object that holds the visual shape properties of the Series. |
| [ShowNegativeBubbles](../../aspose.cells.charts/series/shownegativebubbles/) { get; set; } | True if negative bubbles are shown for the chart group. Valid only for bubble charts. |
| [SizeRepresents](../../aspose.cells.charts/series/sizerepresents/) { get; set; } | Gets or sets what the bubble size represents on a bubble chart. |
| [Smooth](../../aspose.cells.charts/series/smooth/) { get; set; } | Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line and scatter connected by lines charts. |
| [SplitType](../../aspose.cells.charts/series/splittype/) { get; set; } | Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. |
| [SplitValue](../../aspose.cells.charts/series/splitvalue/) { get; set; } | Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. |
| [TrendLines](../../aspose.cells.charts/series/trendlines/) { get; } | Returns all the trendlines of this series. |
| [Type](../../aspose.cells.charts/series/type/) { get; set; } | Gets or sets a data series' type. |
| [UpBars](../../aspose.cells.charts/series/upbars/) { get; } | Returns an DropBars object that represents the up bars on a line chart. Applies only to line charts. |
| [Values](../../aspose.cells.charts/series/values/) { get; set; } | Represents the Y values of this chart series. |
| [ValuesFormatCode](../../aspose.cells.charts/series/valuesformatcode/) { get; set; } | Represents format code of Values's NumberList. |
| [XErrorBar](../../aspose.cells.charts/series/xerrorbar/) { get; } | Represents X direction error bar of the series. |
| [XValues](../../aspose.cells.charts/series/xvalues/) { get; set; } | Represents the x values of the chart series. |
| [XValuesFormatCode](../../aspose.cells.charts/series/xvaluesformatcode/) { get; set; } | Represents format code of X Values's NumberList. |
| [YErrorBar](../../aspose.cells.charts/series/yerrorbar/) { get; } | Represents Y direction error bar of the series. |

## Methods

| Name | Description |
| --- | --- |
| [Move](../../aspose.cells.charts/series/move/)(int) | Moves the series up or down. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesDemo
    {
        public static void SeriesExample()
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
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            // Setting the data source for the category data of NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Accessing the series
            Series series = chart.NSeries[seriesIndex];

            // Setting the values of the series
            series.Values = "=B1:B4";
            // Changing the chart type of the series
            series.Type = ChartType.Line;
            // Setting marker properties
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.ForegroundColorSetType = FormattingType.Automatic;
            series.Marker.ForegroundColor = System.Drawing.Color.Black;
            series.Marker.BackgroundColorSetType = FormattingType.Automatic;

            // Setting additional properties
            series.Name = "First Series";
            series.IsFiltered = false;
            series.ValuesFormatCode = "0.00";
            series.XValues = "=A1:A4";
            series.BubbleSizes = "=B1:B4";
            series.Smooth = true;
            series.Shadow = true;
            series.Has3DEffect = true;
            series.Bar3DShapeType = Bar3DShapeType.Cylinder;
            series.PlotOnSecondAxis = false;
            series.HasHiLoLines = false;
            series.HasSeriesLines = false;
            series.HasDropLines = false;
            series.HasUpDownBars = false;
            series.IsColorVaried = false;
            series.GapWidth = 150;
            series.FirstSliceAngle = 45;
            series.Overlap = 0;
            series.SecondPlotSize = 100;
            series.SplitType = ChartSplitType.Position;
            series.SplitValue = 10.0;
            series.BubbleScale = 100;
            series.SizeRepresents = BubbleSizeRepresents.SizeIsArea;
            series.ShowNegativeBubbles = true;
            series.DoughnutHoleSize = 50;
            series.Explosion = 10;
            series.HasRadarAxisLabels = false;
            series.HasLeaderLines = true;

            // Saving the Excel file
            workbook.Save("SeriesExample.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


