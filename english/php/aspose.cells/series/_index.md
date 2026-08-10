---
title: "Series Class"
linktitle: "Series"
articleTitle: "Series"
second_title: "Aspose.Cells for PHP via Java"
description: "Encapsulates the object that represents a single data series in a chart."
type: docs
weight: 5730
url: /php/aspose.cells/series/
---

## Series class

Encapsulates the object that represents a single data series in a chart.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [IsFiltered](#isfiltered) | boolean | Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be display |
| [LayoutProperties](#layoutproperties) | SeriesLayoutProperties | Represents the properties of layout. |
| [Points](#points) | ChartPointCollection | Gets the collection of points in a series in a chart. When the chart is Pie of Pie or Bar of Pie, the last point is othe |
| [Area](#area) | Area | Represents the background area of Series object. |
| [Border](#border) | Line | Represents border of Series object. |
| [Name](#name) | String | Gets or sets the name of the data series. |
| [DisplayName](#displayname) | String | Gets the series's name that displays on the chart graph. |
| [CountOfDataValues](#countofdatavalues) | Number | Gets the number of the data values. |
| [IsVerticalValues](#isverticalvalues) | boolean | Indicates whether the data source is vertical. |
| [Values](#values) | String | Represents the Y values of this chart series. |
| [CachedValues](#cachedvalues) | ArrayList |  |
| [CachedCategoryValues](#cachedcategoryvalues) | ArrayList |  |
| [PointValues](#pointvalues) | ChartDataValue[] |  |
| [CategoryValues](#categoryvalues) | ChartDataValue[][] |  |
| [ValuesFormatCode](#valuesformatcode) | String | Represents format code of Values's NumberList. |
| [XValuesFormatCode](#xvaluesformatcode) | String | Represents format code of X Values's NumberList. |
| [XValues](#xvalues) | String | Represents the x values of the chart series. |
| [BubbleSizes](#bubblesizes) | String | Gets or sets the bubble sizes values of the chart series. |
| [TrendLines](#trendlines) | TrendlineCollection | Returns all the trendlines of this series. |
| [Smooth](#smooth) | boolean | Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to li |
| [Shadow](#shadow) | boolean | True if the series has a shadow. |
| [Has3DEffect](#has3deffect) | boolean | True if the series has a three-dimensional appearance. Applies only to bubble charts. |
| [Bar3DShapeType](#bar3dshapetype) | Number | Gets or sets the 3D shape type used with the 3-D bar or column chart. The value of the property is Bar3DShapeType intege |
| [DataLabels](#datalabels) | DataLabels | Represents the DataLabels object for the specified ASeries. |
| [Type](#type) | Number | Gets or sets a data series' type. The value of the property is ChartType integer constant. |
| [Marker](#marker) | Marker | Gets the Marker . |
| [PlotOnSecondAxis](#plotonsecondaxis) | boolean | Indicates if this series is plotted on second value axis. |
| [XErrorBar](#xerrorbar) | ErrorBar | Represents X direction error bar of the series. |
| [YErrorBar](#yerrorbar) | ErrorBar | Represents Y direction error bar of the series. |
| [HasHiLoLines](#hashilolines) | boolean | True if the line chart has high-low lines. Applies only to line charts. |
| [HiLoLines](#hilolines) | Line | Returns a HiLoLines object that represents the high-low lines for a series on a line chart. Applies only to line charts. |
| [HasSeriesLines](#hasserieslines) | boolean | True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector  |
| [SeriesLines](#serieslines) | Line | Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. Applies |
| [HasDropLines](#hasdroplines) | boolean | True if the chart has drop lines. Applies only to line chart or area charts. |
| [DropLines](#droplines) | Line | Returns a Line object that represents the drop lines for a series on the line chart or area chart. Applies only to line  |
| [HasUpDownBars](#hasupdownbars) | boolean | True if a line chart has up and down bars. Applies only to line charts. |
| [UpBars](#upbars) | DropBars | Returns an DropBars object that represents the up bars on a line chart. Applies only to line charts. |
| [DownBars](#downbars) | DropBars | Returns a DropBars object that represents the down bars on a line chart. Applies only to line charts. |
| [IsColorVaried](#iscolorvaried) | boolean | Represents if the color of points is varied. The chart must contain only one series. |
| [GapWidth](#gapwidth) | Number | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this  |
| [FirstSliceAngle](#firstsliceangle) | Number | Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies onl |
| [Overlap](#overlap) | Number | Specifies how bars and columns are positioned. Can be a value between – 100 and 100. Applies only to 2-D bar and 2-D col |
| [SecondPlotSize](#secondplotsize) | Number | Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of |
| [SplitType](#splittype) | Number | Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of p |
| [SplitValue](#splitvalue) | Number | Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie o |
| [IsAutoSplit](#isautosplit) | boolean | Indicates whether the threshold value is automatic. |
| [BubbleScale](#bubblescale) | Number | Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, |
| [SizeRepresents](#sizerepresents) | Number | Gets or sets what the bubble size represents on a bubble chart. The value of the property is BubbleSizeRepresents intege |
| [ShowNegativeBubbles](#shownegativebubbles) | boolean | True if negative bubbles are shown for the chart group. Valid only for bubble charts. |
| [DoughnutHoleSize](#doughnutholesize) | Number | Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart  |
| [Explosion](#explosion) | Number | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [HasRadarAxisLabels](#hasradaraxislabels) | boolean | True if a radar chart has category axis labels. Applies only to radar charts. |
| [HasLeaderLines](#hasleaderlines) | boolean | True if the series has leader lines. |
| [LeaderLines](#leaderlines) | Line | Represents leader lines on a chart. Leader lines connect data labels to data points. This object isn’t a collection; the |
| [LegendEntry](#legendentry) | LegendEntry | Gets the legend entry according to this series. |
| [ShapeProperties](#shapeproperties) | ShapePropertyCollection | Gets the ShapePropertyCollection object that holds the visual shape properties of the Series. |
| [BubbleSizeRepresents](#bubblesizerepresents) | Number | Gets what the bubble size represents on a bubble chart. The value of the property is BubbleSizeRepresents integer consta |

## Methods

| Name | Description |
| --- | --- |
| [move](#move) | Moves the series up or down. |

### Series.IsFiltered property {#isfiltered}

Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart.

**Type:** boolean

### Series.LayoutProperties property {#layoutproperties}

Represents the properties of layout.

**Type:** SeriesLayoutProperties

### Series.Points property {#points}

Gets the collection of points in a series in a chart. When the chart is Pie of Pie or Bar of Pie, the last point is other point in first pie plot.

**Type:** ChartPointCollection

### Series.Area property {#area}

Represents the background area of Series object.

**Type:** Area

### Series.Border property {#border}

Represents border of Series object.

**Type:** Line

### Series.Name property {#name}

Gets or sets the name of the data series.

**Type:** String

### Series.DisplayName property {#displayname}

Gets the series's name that displays on the chart graph.

**Type:** String

### Series.CountOfDataValues property {#countofdatavalues}

Gets the number of the data values.

**Type:** Number

### Series.IsVerticalValues property {#isverticalvalues}

Indicates whether the data source is vertical.

**Type:** boolean

### Series.Values property {#values}

Represents the Y values of this chart series.

**Type:** String

### Series.CachedValues property {#cachedvalues}

**Type:** ArrayList

### Series.CachedCategoryValues property {#cachedcategoryvalues}

**Type:** ArrayList

### Series.PointValues property {#pointvalues}

**Type:** ChartDataValue[]

### Series.CategoryValues property {#categoryvalues}

**Type:** ChartDataValue[][]

### Series.ValuesFormatCode property {#valuesformatcode}

Represents format code of Values's NumberList.

**Type:** String

### Series.XValuesFormatCode property {#xvaluesformatcode}

Represents format code of X Values's NumberList.

**Type:** String

### Series.XValues property {#xvalues}

Represents the x values of the chart series.

**Type:** String

### Series.BubbleSizes property {#bubblesizes}

Gets or sets the bubble sizes values of the chart series.

**Type:** String

### Series.TrendLines property {#trendlines}

Returns all the trendlines of this series.

**Type:** TrendlineCollection

### Series.Smooth property {#smooth}

Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line and scatter connected by lines charts.

**Type:** boolean

### Series.Shadow property {#shadow}

True if the series has a shadow.

**Type:** boolean

### Series.Has3DEffect property {#has3deffect}

True if the series has a three-dimensional appearance. Applies only to bubble charts.

**Type:** boolean

### Series.Bar3DShapeType property {#bar3dshapetype}

Gets or sets the 3D shape type used with the 3-D bar or column chart. The value of the property is Bar3DShapeType integer constant.

**Type:** Number

### Series.DataLabels property {#datalabels}

Represents the DataLabels object for the specified ASeries.

**Type:** DataLabels

### Series.Type property {#type}

Gets or sets a data series' type. The value of the property is ChartType integer constant.

**Type:** Number

### Series.Marker property {#marker}

Gets the Marker .

**Type:** Marker

### Series.PlotOnSecondAxis property {#plotonsecondaxis}

Indicates if this series is plotted on second value axis.

**Type:** boolean

### Series.XErrorBar property {#xerrorbar}

Represents X direction error bar of the series.

**Type:** ErrorBar

### Series.YErrorBar property {#yerrorbar}

Represents Y direction error bar of the series.

**Type:** ErrorBar

### Series.HasHiLoLines property {#hashilolines}

True if the line chart has high-low lines. Applies only to line charts.

**Type:** boolean

### Series.HiLoLines property {#hilolines}

Returns a HiLoLines object that represents the high-low lines for a series on a line chart. Applies only to line charts.

**Type:** Line

### Series.HasSeriesLines property {#hasserieslines}

True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts.

**Type:** boolean

### Series.SeriesLines property {#serieslines}

Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. Applies only to stacked bar and stacked column charts.

**Type:** Line

### Series.HasDropLines property {#hasdroplines}

True if the chart has drop lines. Applies only to line chart or area charts.

**Type:** boolean

### Series.DropLines property {#droplines}

Returns a Line object that represents the drop lines for a series on the line chart or area chart. Applies only to line chart or area charts.

**Type:** Line

### Series.HasUpDownBars property {#hasupdownbars}

True if a line chart has up and down bars. Applies only to line charts.

**Type:** boolean

### Series.UpBars property {#upbars}

Returns an DropBars object that represents the up bars on a line chart. Applies only to line charts.

**Type:** DropBars

### Series.DownBars property {#downbars}

Returns a DropBars object that represents the down bars on a line chart. Applies only to line charts.

**Type:** DropBars

### Series.IsColorVaried property {#iscolorvaried}

Represents if the color of points is varied. The chart must contain only one series.

**Type:** boolean

### Series.GapWidth property {#gapwidth}

Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500.

**Type:** Number

### Series.FirstSliceAngle property {#firstsliceangle}

Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.

**Type:** Number

### Series.Overlap property {#overlap}

Specifies how bars and columns are positioned. Can be a value between – 100 and 100. Applies only to 2-D bar and 2-D column charts.

**Type:** Number

### Series.SecondPlotSize property {#secondplotsize}

Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of the size of the primary pie. Can be a value from 5 to 200.

**Type:** Number

### Series.SplitType property {#splittype}

Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. The value of the property is ChartSplitType integer constant.

**Type:** Number

### Series.SplitValue property {#splitvalue}

Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.

**Type:** Number

### Series.IsAutoSplit property {#isautosplit}

Indicates whether the threshold value is automatic.

**Type:** boolean

### Series.BubbleScale property {#bubblescale}

Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, corresponding to a percentage of the default size. Applies only to bubble charts.

**Type:** Number

### Series.SizeRepresents property {#sizerepresents}

Gets or sets what the bubble size represents on a bubble chart. The value of the property is BubbleSizeRepresents integer constant. BubbleSizeRepresents.SizeIsArea means the value BubbleSizes is the area of the bubble. BubbleSizeRepresents.SizeIsWidth means the value BubbleSizes is the width of the bubble.

**Type:** Number

### Series.ShowNegativeBubbles property {#shownegativebubbles}

True if negative bubbles are shown for the chart group. Valid only for bubble charts.

**Type:** boolean

### Series.DoughnutHoleSize property {#doughnutholesize}

Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart size, between 10 and 90 percent.

**Type:** Number

### Series.Explosion property {#explosion}

The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.

**Type:** Number

### Series.HasRadarAxisLabels property {#hasradaraxislabels}

True if a radar chart has category axis labels. Applies only to radar charts.

**Type:** boolean

### Series.HasLeaderLines property {#hasleaderlines}

True if the series has leader lines.

**Type:** boolean

### Series.LeaderLines property {#leaderlines}

Represents leader lines on a chart. Leader lines connect data labels to data points. This object isn’t a collection; there’s no object that represents a single leader line.

**Type:** Line

### Series.LegendEntry property {#legendentry}

Gets the legend entry according to this series.

**Type:** LegendEntry

### Series.ShapeProperties property {#shapeproperties}

Gets the ShapePropertyCollection object that holds the visual shape properties of the Series.

**Type:** ShapePropertyCollection

### Series.BubbleSizeRepresents property {#bubblesizerepresents}

Gets what the bubble size represents on a bubble chart. The value of the property is BubbleSizeRepresents integer constant. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Charts.Series.SizeRepresents property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Type:** Number

### move(count) {#move}

Moves the series up or down.

| Parameter | Type | Description |
| --- | --- | --- |
| count | Number | The number of moving up or down. Move the series up if this is less than zero; Move the series down if this is greater than zero. |
