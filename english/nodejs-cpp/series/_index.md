---
title: Series
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents a single data series in a chart.
type: docs
url: /nodejs-cpp/series/
---

## Series class

Encapsulates the object that represents a single data series in a chart.

```javascript
class Series;
```


### Example
```javascript
const { Workbook, ChartType, ChartMarkerType, FormattingType, Color } = require("aspose.cells.node");

//Instantiating a Workbook object
var workbook = new Workbook();
//Adding a new worksheet to the Excel object
var sheetIndex = workbook.worksheets.add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
var worksheet = workbook.worksheets.get(sheetIndex);
//Adding a sample value to "A1" cell
worksheet.cells.get("A1").putValue(50);
//Adding a sample value to "A2" cell
worksheet.cells.get("A2").putValue(100);
//Adding a sample value to "A3" cell
worksheet.cells.get("A3").putValue(150);
//Adding a sample value to "A4" cell
worksheet.cells.get("A4").putValue(200);
//Adding a sample value to "B1" cell
worksheet.cells.get("B1").putValue(60);
//Adding a sample value to "B2" cell
worksheet.cells.get("B2").putValue(32);
//Adding a sample value to "B3" cell
worksheet.cells.get("B3").putValue(50);
//Adding a sample value to "B4" cell
worksheet.cells.get("B4").putValue(40);
//Adding a sample value to "C1" cell as category data
worksheet.cells.get("C1").putValue("Q1");
//Adding a sample value to "C2" cell as category data
worksheet.cells.get("C2").putValue("Q2");
//Adding a sample value to "C3" cell as category data
worksheet.cells.get("C3").putValue("Y1");
//Adding a sample value to "C4" cell as category data
worksheet.cells.get("C4").putValue("Y2");
//Adding a chart to the worksheet
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Accessing the instance of the newly added chart
var chart = worksheet.charts.get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.nSeries.add("A1:B4", true);
//Setting the data source for the category data of NSeries
chart.nSeries.categoryData = "C1:C4";
var series = chart.nSeries.get(1);
//Setting the values of the series.
series.values = "=B1:B4";
//Changing the chart type of the series.
series.type = ChartType.Line;
//Setting marker properties.
series.marker.markerStyle = ChartMarkerType.Circle;
series.marker.foregroundColorSetType = FormattingType.Automatic;
series.marker.foregroundColor = Color.Black;
series.marker.backgroundColorSetType = FormattingType.Automatic;
//Saving the Excel file
workbook.save("output/ChartsSeries.xls");
```
## Properties

| Property | Type | Description |
| --- | --- | --- |
| [isFiltered](#isFiltered--)| boolean | Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart. |
| [layoutProperties](#layoutProperties--)| SeriesLayoutProperties | Readonly. Represents the properties of layout. |
| [points](#points--)| ChartPointCollection | Readonly. Gets the collection of points in a series in a chart. |
| [area](#area--)| Area | Readonly. Represents the background area of Series object. |
| [border](#border--)| Line | Readonly. Represents border of Series object. |
| [name](#name--)| string | Gets or sets the name of the data series. |
| [displayName](#displayName--)| string | Readonly. Gets the series's name that displays on the chart graph. |
| [countOfDataValues](#countOfDataValues--)| number | Readonly. Gets the number of the data values. |
| [isVerticalValues](#isVerticalValues--)| boolean | Readonly. Indicates whether the data source is vertical. |
| [values](#values--)| string | Represents the Y values of this chart series. |
| [pointValues](#pointValues--)| ChartDataValue[] | Readonly. Gets the values for the points of the series |
| [categoryValues](#categoryValues--)| ChartDataValue[][] | Readonly. Gets the category values of the series |
| [valuesFormatCode](#valuesFormatCode--)| string | Represents format code of Values's NumberList. |
| [xValuesFormatCode](#xValuesFormatCode--)| string | Represents format code of X Values's NumberList. |
| [xValues](#xValues--)| string | Represents the x values of the chart series. |
| [bubbleSizes](#bubbleSizes--)| string | Gets or sets the bubble sizes values of the chart series. |
| [trendLines](#trendLines--)| TrendlineCollection | Readonly. Returns all the trendlines of this series. |
| [smooth](#smooth--)| boolean | Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line and scatter connected by lines charts. |
| [shadow](#shadow--)| boolean | True if the series has a shadow. |
| [has3DEffect](#has3DEffect--)| boolean | True if the series has a three-dimensional appearance. Applies only to bubble charts. |
| [bar3DShapeType](#bar3DShapeType--)| Bar3DShapeType | Gets or sets the 3D shape type used with the 3-D bar or column chart. |
| [dataLabels](#dataLabels--)| DataLabels | Readonly. Represents the DataLabels object for the specified ASeries. |
| [type](#type--)| ChartType | Gets or sets a data series' type. |
| [marker](#marker--)| Marker | Readonly. Gets the <see cref="Marker">marker</see>. |
| [plotOnSecondAxis](#plotOnSecondAxis--)| boolean | Indicates if this series is plotted on second value axis. |
| [xErrorBar](#xErrorBar--)| ErrorBar | Readonly. Represents X direction error bar of the series. |
| [yErrorBar](#yErrorBar--)| ErrorBar | Readonly. Represents Y direction error bar of the series. |
| [hasHiLoLines](#hasHiLoLines--)| boolean | True if the line chart has high-low lines. Applies only to line charts. |
| [hiLoLines](#hiLoLines--)| Line | Readonly. Returns a HiLoLines object that represents the high-low lines for a series on a line chart. Applies only to line charts. |
| [hasSeriesLines](#hasSeriesLines--)| boolean | True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts. |
| [seriesLines](#seriesLines--)| Line | Readonly. Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. Applies only to stacked bar and stacked column charts. |
| [hasDropLines](#hasDropLines--)| boolean | True if the chart has drop lines. Applies only to line chart or area charts. |
| [dropLines](#dropLines--)| Line | Readonly. Returns a [Line](../line/) object that represents the drop lines for a series on the line chart or area chart. Applies only to line chart or area charts. |
| [hasUpDownBars](#hasUpDownBars--)| boolean | True if a line chart has up and down bars. Applies only to line charts. |
| [upBars](#upBars--)| DropBars | Readonly. Returns an DropBars object that represents the up bars on a line chart. Applies only to line charts. |
| [downBars](#downBars--)| DropBars | Readonly. Returns a [DropBars](../dropbars/) object that represents the down bars on a line chart. Applies only to line charts. |
| [isColorVaried](#isColorVaried--)| boolean | Represents if the color of points is varied. The chart must contain only one series. |
| [gapWidth](#gapWidth--)| number | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500. |
| [firstSliceAngle](#firstSliceAngle--)| number | Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360. |
| [overlap](#overlap--)| number | Specifies how bars and columns are positioned. Can be a value between – 100 and 100. Applies only to 2-D bar and 2-D column charts. |
| [secondPlotSize](#secondPlotSize--)| number | Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of the size of the primary pie. Can be a value from 5 to 200. |
| [splitType](#splitType--)| ChartSplitType | Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. |
| [splitValue](#splitValue--)| number | Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. |
| [isAutoSplit](#isAutoSplit--)| boolean | Readonly. Indicates whether the threshold value is automatic. |
| [bubbleScale](#bubbleScale--)| number | Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, corresponding to a percentage of the default size. Applies only to bubble charts. |
| [sizeRepresents](#sizeRepresents--)| BubbleSizeRepresents | Gets or sets what the bubble size represents on a bubble chart. |
| [showNegativeBubbles](#showNegativeBubbles--)| boolean | True if negative bubbles are shown for the chart group. Valid only for bubble charts. |
| [doughnutHoleSize](#doughnutHoleSize--)| number | Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart size, between 10 and 90 percent. |
| [explosion](#explosion--)| number | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [hasRadarAxisLabels](#hasRadarAxisLabels--)| boolean | True if a radar chart has category axis labels. Applies only to radar charts. |
| [hasLeaderLines](#hasLeaderLines--)| boolean | True if the series has leader lines. |
| [leaderLines](#leaderLines--)| Line | Readonly. Represents leader lines on a chart. Leader lines connect data labels to data points. This object isn’t a collection; there’s no object that represents a single leader line. |
| [legendEntry](#legendEntry--)| LegendEntry | Readonly. Gets the legend entry according to this series. |
| [shapeProperties](#shapeProperties--)| ShapePropertyCollection | Readonly. Gets the [ShapePropertyCollection](../shapepropertycollection/) object that holds the visual shape properties of the Series. |

## Methods

| Method | Description |
| --- | --- |
| [isFiltered()](#isFiltered--)| <b>@deprecated.</b> Please use the 'isFiltered' property instead. Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart. |
| [setIsFiltered(boolean)](#setIsFiltered-boolean-)| <b>@deprecated.</b> Please use the 'isFiltered' property instead. Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart. |
| [getLayoutProperties()](#getLayoutProperties--)| <b>@deprecated.</b> Please use the 'layoutProperties' property instead. Represents the properties of layout. |
| [getPoints()](#getPoints--)| <b>@deprecated.</b> Please use the 'points' property instead. Gets the collection of points in a series in a chart. |
| [getArea()](#getArea--)| <b>@deprecated.</b> Please use the 'area' property instead. Represents the background area of Series object. |
| [getBorder()](#getBorder--)| <b>@deprecated.</b> Please use the 'border' property instead. Represents border of Series object. |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets or sets the name of the data series. |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Gets or sets the name of the data series. |
| [getDisplayName()](#getDisplayName--)| <b>@deprecated.</b> Please use the 'displayName' property instead. Gets the series's name that displays on the chart graph. |
| [getCountOfDataValues()](#getCountOfDataValues--)| <b>@deprecated.</b> Please use the 'countOfDataValues' property instead. Gets the number of the data values. |
| [isVerticalValues()](#isVerticalValues--)| <b>@deprecated.</b> Please use the 'isVerticalValues' property instead. Indicates whether the data source is vertical. |
| [getValues()](#getValues--)| <b>@deprecated.</b> Please use the 'values' property instead. Represents the Y values of this chart series. |
| [setValues(string)](#setValues-string-)| <b>@deprecated.</b> Please use the 'values' property instead. Represents the Y values of this chart series. |
| [getPointValues()](#getPointValues--)| <b>@deprecated.</b> Please use the 'pointValues' property instead. Gets the values for the points of the series |
| [getCategoryValues()](#getCategoryValues--)| <b>@deprecated.</b> Please use the 'categoryValues' property instead. Gets the category values of the series |
| [getValuesFormatCode()](#getValuesFormatCode--)| <b>@deprecated.</b> Please use the 'valuesFormatCode' property instead. Represents format code of Values's NumberList. |
| [setValuesFormatCode(string)](#setValuesFormatCode-string-)| <b>@deprecated.</b> Please use the 'valuesFormatCode' property instead. Represents format code of Values's NumberList. |
| [getXValuesFormatCode()](#getXValuesFormatCode--)| <b>@deprecated.</b> Please use the 'xValuesFormatCode' property instead. Represents format code of X Values's NumberList. |
| [setXValuesFormatCode(string)](#setXValuesFormatCode-string-)| <b>@deprecated.</b> Please use the 'xValuesFormatCode' property instead. Represents format code of X Values's NumberList. |
| [getXValues()](#getXValues--)| <b>@deprecated.</b> Please use the 'xValues' property instead. Represents the x values of the chart series. |
| [setXValues(string)](#setXValues-string-)| <b>@deprecated.</b> Please use the 'xValues' property instead. Represents the x values of the chart series. |
| [getBubbleSizes()](#getBubbleSizes--)| <b>@deprecated.</b> Please use the 'bubbleSizes' property instead. Gets or sets the bubble sizes values of the chart series. |
| [setBubbleSizes(string)](#setBubbleSizes-string-)| <b>@deprecated.</b> Please use the 'bubbleSizes' property instead. Gets or sets the bubble sizes values of the chart series. |
| [getTrendLines()](#getTrendLines--)| <b>@deprecated.</b> Please use the 'trendLines' property instead. Returns all the trendlines of this series. |
| [getSmooth()](#getSmooth--)| <b>@deprecated.</b> Please use the 'smooth' property instead. Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line and scatter connected by lines charts. |
| [setSmooth(boolean)](#setSmooth-boolean-)| <b>@deprecated.</b> Please use the 'smooth' property instead. Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line and scatter connected by lines charts. |
| [getShadow()](#getShadow--)| <b>@deprecated.</b> Please use the 'shadow' property instead. True if the series has a shadow. |
| [setShadow(boolean)](#setShadow-boolean-)| <b>@deprecated.</b> Please use the 'shadow' property instead. True if the series has a shadow. |
| [getHas3DEffect()](#getHas3DEffect--)| <b>@deprecated.</b> Please use the 'has3DEffect' property instead. True if the series has a three-dimensional appearance. Applies only to bubble charts. |
| [setHas3DEffect(boolean)](#setHas3DEffect-boolean-)| <b>@deprecated.</b> Please use the 'has3DEffect' property instead. True if the series has a three-dimensional appearance. Applies only to bubble charts. |
| [getBar3DShapeType()](#getBar3DShapeType--)| <b>@deprecated.</b> Please use the 'bar3DShapeType' property instead. Gets or sets the 3D shape type used with the 3-D bar or column chart. |
| [setBar3DShapeType(Bar3DShapeType)](#setBar3DShapeType-bar3dshapetype-)| <b>@deprecated.</b> Please use the 'bar3DShapeType' property instead. Gets or sets the 3D shape type used with the 3-D bar or column chart. |
| [getDataLabels()](#getDataLabels--)| <b>@deprecated.</b> Please use the 'dataLabels' property instead. Represents the DataLabels object for the specified ASeries. |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets or sets a data series' type. |
| [setType(ChartType)](#setType-charttype-)| <b>@deprecated.</b> Please use the 'type' property instead. Gets or sets a data series' type. |
| [getMarker()](#getMarker--)| <b>@deprecated.</b> Please use the 'marker' property instead. Gets the <see cref="Marker">marker</see>. |
| [getPlotOnSecondAxis()](#getPlotOnSecondAxis--)| <b>@deprecated.</b> Please use the 'plotOnSecondAxis' property instead. Indicates if this series is plotted on second value axis. |
| [setPlotOnSecondAxis(boolean)](#setPlotOnSecondAxis-boolean-)| <b>@deprecated.</b> Please use the 'plotOnSecondAxis' property instead. Indicates if this series is plotted on second value axis. |
| [getXErrorBar()](#getXErrorBar--)| <b>@deprecated.</b> Please use the 'xErrorBar' property instead. Represents X direction error bar of the series. |
| [getYErrorBar()](#getYErrorBar--)| <b>@deprecated.</b> Please use the 'yErrorBar' property instead. Represents Y direction error bar of the series. |
| [getHasHiLoLines()](#getHasHiLoLines--)| <b>@deprecated.</b> Please use the 'hasHiLoLines' property instead. True if the line chart has high-low lines. Applies only to line charts. |
| [setHasHiLoLines(boolean)](#setHasHiLoLines-boolean-)| <b>@deprecated.</b> Please use the 'hasHiLoLines' property instead. True if the line chart has high-low lines. Applies only to line charts. |
| [getHiLoLines()](#getHiLoLines--)| <b>@deprecated.</b> Please use the 'hiLoLines' property instead. Returns a HiLoLines object that represents the high-low lines for a series on a line chart. Applies only to line charts. |
| [getHasSeriesLines()](#getHasSeriesLines--)| <b>@deprecated.</b> Please use the 'hasSeriesLines' property instead. True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts. |
| [setHasSeriesLines(boolean)](#setHasSeriesLines-boolean-)| <b>@deprecated.</b> Please use the 'hasSeriesLines' property instead. True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts. |
| [getSeriesLines()](#getSeriesLines--)| <b>@deprecated.</b> Please use the 'seriesLines' property instead. Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. Applies only to stacked bar and stacked column charts. |
| [getHasDropLines()](#getHasDropLines--)| <b>@deprecated.</b> Please use the 'hasDropLines' property instead. True if the chart has drop lines. Applies only to line chart or area charts. |
| [setHasDropLines(boolean)](#setHasDropLines-boolean-)| <b>@deprecated.</b> Please use the 'hasDropLines' property instead. True if the chart has drop lines. Applies only to line chart or area charts. |
| [getDropLines()](#getDropLines--)| <b>@deprecated.</b> Please use the 'dropLines' property instead. Returns a [Line](../line/) object that represents the drop lines for a series on the line chart or area chart. Applies only to line chart or area charts. |
| [getHasUpDownBars()](#getHasUpDownBars--)| <b>@deprecated.</b> Please use the 'hasUpDownBars' property instead. True if a line chart has up and down bars. Applies only to line charts. |
| [setHasUpDownBars(boolean)](#setHasUpDownBars-boolean-)| <b>@deprecated.</b> Please use the 'hasUpDownBars' property instead. True if a line chart has up and down bars. Applies only to line charts. |
| [getUpBars()](#getUpBars--)| <b>@deprecated.</b> Please use the 'upBars' property instead. Returns an DropBars object that represents the up bars on a line chart. Applies only to line charts. |
| [getDownBars()](#getDownBars--)| <b>@deprecated.</b> Please use the 'downBars' property instead. Returns a [DropBars](../dropbars/) object that represents the down bars on a line chart. Applies only to line charts. |
| [isColorVaried()](#isColorVaried--)| <b>@deprecated.</b> Please use the 'isColorVaried' property instead. Represents if the color of points is varied. The chart must contain only one series. |
| [setIsColorVaried(boolean)](#setIsColorVaried-boolean-)| <b>@deprecated.</b> Please use the 'isColorVaried' property instead. Represents if the color of points is varied. The chart must contain only one series. |
| [getGapWidth()](#getGapWidth--)| <b>@deprecated.</b> Please use the 'gapWidth' property instead. Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500. |
| [setGapWidth(number)](#setGapWidth-number-)| <b>@deprecated.</b> Please use the 'gapWidth' property instead. Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500. |
| [getFirstSliceAngle()](#getFirstSliceAngle--)| <b>@deprecated.</b> Please use the 'firstSliceAngle' property instead. Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360. |
| [setFirstSliceAngle(number)](#setFirstSliceAngle-number-)| <b>@deprecated.</b> Please use the 'firstSliceAngle' property instead. Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360. |
| [getOverlap()](#getOverlap--)| <b>@deprecated.</b> Please use the 'overlap' property instead. Specifies how bars and columns are positioned. Can be a value between – 100 and 100. Applies only to 2-D bar and 2-D column charts. |
| [setOverlap(number)](#setOverlap-number-)| <b>@deprecated.</b> Please use the 'overlap' property instead. Specifies how bars and columns are positioned. Can be a value between – 100 and 100. Applies only to 2-D bar and 2-D column charts. |
| [getSecondPlotSize()](#getSecondPlotSize--)| <b>@deprecated.</b> Please use the 'secondPlotSize' property instead. Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of the size of the primary pie. Can be a value from 5 to 200. |
| [setSecondPlotSize(number)](#setSecondPlotSize-number-)| <b>@deprecated.</b> Please use the 'secondPlotSize' property instead. Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of the size of the primary pie. Can be a value from 5 to 200. |
| [getSplitType()](#getSplitType--)| <b>@deprecated.</b> Please use the 'splitType' property instead. Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. |
| [setSplitType(ChartSplitType)](#setSplitType-chartsplittype-)| <b>@deprecated.</b> Please use the 'splitType' property instead. Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. |
| [getSplitValue()](#getSplitValue--)| <b>@deprecated.</b> Please use the 'splitValue' property instead. Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. |
| [setSplitValue(number)](#setSplitValue-number-)| <b>@deprecated.</b> Please use the 'splitValue' property instead. Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. |
| [isAutoSplit()](#isAutoSplit--)| <b>@deprecated.</b> Please use the 'isAutoSplit' property instead. Indicates whether the threshold value is automatic. |
| [getBubbleScale()](#getBubbleScale--)| <b>@deprecated.</b> Please use the 'bubbleScale' property instead. Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, corresponding to a percentage of the default size. Applies only to bubble charts. |
| [setBubbleScale(number)](#setBubbleScale-number-)| <b>@deprecated.</b> Please use the 'bubbleScale' property instead. Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, corresponding to a percentage of the default size. Applies only to bubble charts. |
| [getSizeRepresents()](#getSizeRepresents--)| <b>@deprecated.</b> Please use the 'sizeRepresents' property instead. Gets or sets what the bubble size represents on a bubble chart. |
| [setSizeRepresents(BubbleSizeRepresents)](#setSizeRepresents-bubblesizerepresents-)| <b>@deprecated.</b> Please use the 'sizeRepresents' property instead. Gets or sets what the bubble size represents on a bubble chart. |
| [getShowNegativeBubbles()](#getShowNegativeBubbles--)| <b>@deprecated.</b> Please use the 'showNegativeBubbles' property instead. True if negative bubbles are shown for the chart group. Valid only for bubble charts. |
| [setShowNegativeBubbles(boolean)](#setShowNegativeBubbles-boolean-)| <b>@deprecated.</b> Please use the 'showNegativeBubbles' property instead. True if negative bubbles are shown for the chart group. Valid only for bubble charts. |
| [getDoughnutHoleSize()](#getDoughnutHoleSize--)| <b>@deprecated.</b> Please use the 'doughnutHoleSize' property instead. Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart size, between 10 and 90 percent. |
| [setDoughnutHoleSize(number)](#setDoughnutHoleSize-number-)| <b>@deprecated.</b> Please use the 'doughnutHoleSize' property instead. Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart size, between 10 and 90 percent. |
| [getExplosion()](#getExplosion--)| <b>@deprecated.</b> Please use the 'explosion' property instead. The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [setExplosion(number)](#setExplosion-number-)| <b>@deprecated.</b> Please use the 'explosion' property instead. The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [getHasRadarAxisLabels()](#getHasRadarAxisLabels--)| <b>@deprecated.</b> Please use the 'hasRadarAxisLabels' property instead. True if a radar chart has category axis labels. Applies only to radar charts. |
| [setHasRadarAxisLabels(boolean)](#setHasRadarAxisLabels-boolean-)| <b>@deprecated.</b> Please use the 'hasRadarAxisLabels' property instead. True if a radar chart has category axis labels. Applies only to radar charts. |
| [getHasLeaderLines()](#getHasLeaderLines--)| <b>@deprecated.</b> Please use the 'hasLeaderLines' property instead. True if the series has leader lines. |
| [setHasLeaderLines(boolean)](#setHasLeaderLines-boolean-)| <b>@deprecated.</b> Please use the 'hasLeaderLines' property instead. True if the series has leader lines. |
| [getLeaderLines()](#getLeaderLines--)| <b>@deprecated.</b> Please use the 'leaderLines' property instead. Represents leader lines on a chart. Leader lines connect data labels to data points. This object isn’t a collection; there’s no object that represents a single leader line. |
| [getLegendEntry()](#getLegendEntry--)| <b>@deprecated.</b> Please use the 'legendEntry' property instead. Gets the legend entry according to this series. |
| [getShapeProperties()](#getShapeProperties--)| <b>@deprecated.</b> Please use the 'shapeProperties' property instead. Gets the [ShapePropertyCollection](../shapepropertycollection/) object that holds the visual shape properties of the Series. |
| [move(number)](#move-number-)| Moves the series up or down. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### isFiltered {#isFiltered--}

Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart.

```javascript
isFiltered : boolean;
```


### layoutProperties {#layoutProperties--}

Readonly. Represents the properties of layout.

```javascript
layoutProperties : SeriesLayoutProperties;
```


### points {#points--}

Readonly. Gets the collection of points in a series in a chart.

```javascript
points : ChartPointCollection;
```


**Remarks**

When the chart is Pie of Pie or Bar of Pie, the last point is other point in first pie plot.

### area {#area--}

Readonly. Represents the background area of Series object.

```javascript
area : Area;
```


### border {#border--}

Readonly. Represents border of Series object.

```javascript
border : Line;
```


### name {#name--}

Gets or sets the name of the data series.

```javascript
name : string;
```


**Example**
```javascript
const { Workbook, ChartType } = require("aspose.cells.node");

var workbook = new Workbook();
//Get the first worksheet.
var worksheet = workbook.worksheets.get(0);
//Adding a chart to the worksheet
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Accessing the instance of the newly added chart
var chart = worksheet.charts.get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.nSeries.add("A1:B4", true);
//Reference name to a cell
chart.nSeries.get(0).name = "=A1";
//Set a string to name
chart.nSeries.get(0).name = "First Series";
```

### displayName {#displayName--}

Readonly. Gets the series's name that displays on the chart graph.

```javascript
displayName : string;
```


### countOfDataValues {#countOfDataValues--}

Readonly. Gets the number of the data values.

```javascript
countOfDataValues : number;
```


### isVerticalValues {#isVerticalValues--}

Readonly. Indicates whether the data source is vertical.

```javascript
isVerticalValues : boolean;
```


### values {#values--}

Represents the Y values of this chart series.

```javascript
values : string;
```


### pointValues {#pointValues--}

Readonly. Gets the values for the points of the series

```javascript
pointValues : ChartDataValue[];
```


### categoryValues {#categoryValues--}

Readonly. Gets the category values of the series

```javascript
categoryValues : ChartDataValue[][];
```


### valuesFormatCode {#valuesFormatCode--}

Represents format code of Values's NumberList.

```javascript
valuesFormatCode : string;
```


### xValuesFormatCode {#xValuesFormatCode--}

Represents format code of X Values's NumberList.

```javascript
xValuesFormatCode : string;
```


### xValues {#xValues--}

Represents the x values of the chart series.

```javascript
xValues : string;
```


### bubbleSizes {#bubbleSizes--}

Gets or sets the bubble sizes values of the chart series.

```javascript
bubbleSizes : string;
```


### trendLines {#trendLines--}

Readonly. Returns all the trendlines of this series.

```javascript
trendLines : TrendlineCollection;
```


### smooth {#smooth--}

Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line and scatter connected by lines charts.

```javascript
smooth : boolean;
```


### shadow {#shadow--}

True if the series has a shadow.

```javascript
shadow : boolean;
```


### has3DEffect {#has3DEffect--}

True if the series has a three-dimensional appearance. Applies only to bubble charts.

```javascript
has3DEffect : boolean;
```


### bar3DShapeType {#bar3DShapeType--}

Gets or sets the 3D shape type used with the 3-D bar or column chart.

```javascript
bar3DShapeType : Bar3DShapeType;
```


### dataLabels {#dataLabels--}

Readonly. Represents the DataLabels object for the specified ASeries.

```javascript
dataLabels : DataLabels;
```


### type {#type--}

Gets or sets a data series' type.

```javascript
type : ChartType;
```


### marker {#marker--}

Readonly. Gets the <see cref="Marker">marker</see>.

```javascript
marker : Marker;
```


### plotOnSecondAxis {#plotOnSecondAxis--}

Indicates if this series is plotted on second value axis.

```javascript
plotOnSecondAxis : boolean;
```


### xErrorBar {#xErrorBar--}

Readonly. Represents X direction error bar of the series.

```javascript
xErrorBar : ErrorBar;
```


### yErrorBar {#yErrorBar--}

Readonly. Represents Y direction error bar of the series.

```javascript
yErrorBar : ErrorBar;
```


### hasHiLoLines {#hasHiLoLines--}

True if the line chart has high-low lines. Applies only to line charts.

```javascript
hasHiLoLines : boolean;
```


### hiLoLines {#hiLoLines--}

Readonly. Returns a HiLoLines object that represents the high-low lines for a series on a line chart. Applies only to line charts.

```javascript
hiLoLines : Line;
```


### hasSeriesLines {#hasSeriesLines--}

True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts.

```javascript
hasSeriesLines : boolean;
```


### seriesLines {#seriesLines--}

Readonly. Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. Applies only to stacked bar and stacked column charts.

```javascript
seriesLines : Line;
```


### hasDropLines {#hasDropLines--}

True if the chart has drop lines. Applies only to line chart or area charts.

```javascript
hasDropLines : boolean;
```


### dropLines {#dropLines--}

Readonly. Returns a [Line](../line/) object that represents the drop lines for a series on the line chart or area chart. Applies only to line chart or area charts.

```javascript
dropLines : Line;
```


### hasUpDownBars {#hasUpDownBars--}

True if a line chart has up and down bars. Applies only to line charts.

```javascript
hasUpDownBars : boolean;
```


### upBars {#upBars--}

Readonly. Returns an DropBars object that represents the up bars on a line chart. Applies only to line charts.

```javascript
upBars : DropBars;
```


### downBars {#downBars--}

Readonly. Returns a [DropBars](../dropbars/) object that represents the down bars on a line chart. Applies only to line charts.

```javascript
downBars : DropBars;
```


### isColorVaried {#isColorVaried--}

Represents if the color of points is varied. The chart must contain only one series.

```javascript
isColorVaried : boolean;
```


### gapWidth {#gapWidth--}

Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500.

```javascript
gapWidth : number;
```


### firstSliceAngle {#firstSliceAngle--}

Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.

```javascript
firstSliceAngle : number;
```


### overlap {#overlap--}

Specifies how bars and columns are positioned. Can be a value between – 100 and 100. Applies only to 2-D bar and 2-D column charts.

```javascript
overlap : number;
```


### secondPlotSize {#secondPlotSize--}

Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of the size of the primary pie. Can be a value from 5 to 200.

```javascript
secondPlotSize : number;
```


### splitType {#splitType--}

Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.

```javascript
splitType : ChartSplitType;
```


### splitValue {#splitValue--}

Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.

```javascript
splitValue : number;
```


### isAutoSplit {#isAutoSplit--}

Readonly. Indicates whether the threshold value is automatic.

```javascript
isAutoSplit : boolean;
```


### bubbleScale {#bubbleScale--}

Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, corresponding to a percentage of the default size. Applies only to bubble charts.

```javascript
bubbleScale : number;
```


### sizeRepresents {#sizeRepresents--}

Gets or sets what the bubble size represents on a bubble chart.

```javascript
sizeRepresents : BubbleSizeRepresents;
```


**Remarks**

BubbleSizeRepresents.SizeIsArea means the value [Series.BubbleSizes](../series.bubblesizes/) is the area of the bubble. BubbleSizeRepresents.SizeIsWidth means the value [Series.BubbleSizes](../series.bubblesizes/) is the width of the bubble.

### showNegativeBubbles {#showNegativeBubbles--}

True if negative bubbles are shown for the chart group. Valid only for bubble charts.

```javascript
showNegativeBubbles : boolean;
```


### doughnutHoleSize {#doughnutHoleSize--}

Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart size, between 10 and 90 percent.

```javascript
doughnutHoleSize : number;
```


### explosion {#explosion--}

The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.

```javascript
explosion : number;
```


### hasRadarAxisLabels {#hasRadarAxisLabels--}

True if a radar chart has category axis labels. Applies only to radar charts.

```javascript
hasRadarAxisLabels : boolean;
```


### hasLeaderLines {#hasLeaderLines--}

True if the series has leader lines.

```javascript
hasLeaderLines : boolean;
```


### leaderLines {#leaderLines--}

Readonly. Represents leader lines on a chart. Leader lines connect data labels to data points. This object isn’t a collection; there’s no object that represents a single leader line.

```javascript
leaderLines : Line;
```


### legendEntry {#legendEntry--}

Readonly. Gets the legend entry according to this series.

```javascript
legendEntry : LegendEntry;
```


### shapeProperties {#shapeProperties--}

Readonly. Gets the [ShapePropertyCollection](../shapepropertycollection/) object that holds the visual shape properties of the Series.

```javascript
shapeProperties : ShapePropertyCollection;
```


### isFiltered() {#isFiltered--}

<b>@deprecated.</b> Please use the 'isFiltered' property instead. Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart.

```javascript
isFiltered() : boolean;
```


### setIsFiltered(boolean) {#setIsFiltered-boolean-}

<b>@deprecated.</b> Please use the 'isFiltered' property instead. Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart.

```javascript
setIsFiltered(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getLayoutProperties() {#getLayoutProperties--}

<b>@deprecated.</b> Please use the 'layoutProperties' property instead. Represents the properties of layout.

```javascript
getLayoutProperties() : SeriesLayoutProperties;
```


**Returns**

[SeriesLayoutProperties](../serieslayoutproperties/)

### getPoints() {#getPoints--}

<b>@deprecated.</b> Please use the 'points' property instead. Gets the collection of points in a series in a chart.

```javascript
getPoints() : ChartPointCollection;
```


**Returns**

[ChartPointCollection](../chartpointcollection/)

**Remarks**

When the chart is Pie of Pie or Bar of Pie, the last point is other point in first pie plot.

### getArea() {#getArea--}

<b>@deprecated.</b> Please use the 'area' property instead. Represents the background area of Series object.

```javascript
getArea() : Area;
```


**Returns**

[Area](../area/)

### getBorder() {#getBorder--}

<b>@deprecated.</b> Please use the 'border' property instead. Represents border of Series object.

```javascript
getBorder() : Line;
```


**Returns**

[Line](../line/)

### getName() {#getName--}

<b>@deprecated.</b> Please use the 'name' property instead. Gets or sets the name of the data series.

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

<b>@deprecated.</b> Please use the 'name' property instead. Gets or sets the name of the data series.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getDisplayName() {#getDisplayName--}

<b>@deprecated.</b> Please use the 'displayName' property instead. Gets the series's name that displays on the chart graph.

```javascript
getDisplayName() : string;
```


### getCountOfDataValues() {#getCountOfDataValues--}

<b>@deprecated.</b> Please use the 'countOfDataValues' property instead. Gets the number of the data values.

```javascript
getCountOfDataValues() : number;
```


### isVerticalValues() {#isVerticalValues--}

<b>@deprecated.</b> Please use the 'isVerticalValues' property instead. Indicates whether the data source is vertical.

```javascript
isVerticalValues() : boolean;
```


### getValues() {#getValues--}

<b>@deprecated.</b> Please use the 'values' property instead. Represents the Y values of this chart series.

```javascript
getValues() : string;
```


### setValues(string) {#setValues-string-}

<b>@deprecated.</b> Please use the 'values' property instead. Represents the Y values of this chart series.

```javascript
setValues(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getPointValues() {#getPointValues--}

<b>@deprecated.</b> Please use the 'pointValues' property instead. Gets the values for the points of the series

```javascript
getPointValues() : ChartDataValue[];
```


**Returns**

[ChartDataValue](../chartdatavalue/)[]

### getCategoryValues() {#getCategoryValues--}

<b>@deprecated.</b> Please use the 'categoryValues' property instead. Gets the category values of the series

```javascript
getCategoryValues() : ChartDataValue[][];
```


**Returns**

[ChartDataValue[]](../chartdatavalue[]/)[]

### getValuesFormatCode() {#getValuesFormatCode--}

<b>@deprecated.</b> Please use the 'valuesFormatCode' property instead. Represents format code of Values's NumberList.

```javascript
getValuesFormatCode() : string;
```


### setValuesFormatCode(string) {#setValuesFormatCode-string-}

<b>@deprecated.</b> Please use the 'valuesFormatCode' property instead. Represents format code of Values's NumberList.

```javascript
setValuesFormatCode(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getXValuesFormatCode() {#getXValuesFormatCode--}

<b>@deprecated.</b> Please use the 'xValuesFormatCode' property instead. Represents format code of X Values's NumberList.

```javascript
getXValuesFormatCode() : string;
```


### setXValuesFormatCode(string) {#setXValuesFormatCode-string-}

<b>@deprecated.</b> Please use the 'xValuesFormatCode' property instead. Represents format code of X Values's NumberList.

```javascript
setXValuesFormatCode(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getXValues() {#getXValues--}

<b>@deprecated.</b> Please use the 'xValues' property instead. Represents the x values of the chart series.

```javascript
getXValues() : string;
```


### setXValues(string) {#setXValues-string-}

<b>@deprecated.</b> Please use the 'xValues' property instead. Represents the x values of the chart series.

```javascript
setXValues(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getBubbleSizes() {#getBubbleSizes--}

<b>@deprecated.</b> Please use the 'bubbleSizes' property instead. Gets or sets the bubble sizes values of the chart series.

```javascript
getBubbleSizes() : string;
```


### setBubbleSizes(string) {#setBubbleSizes-string-}

<b>@deprecated.</b> Please use the 'bubbleSizes' property instead. Gets or sets the bubble sizes values of the chart series.

```javascript
setBubbleSizes(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getTrendLines() {#getTrendLines--}

<b>@deprecated.</b> Please use the 'trendLines' property instead. Returns all the trendlines of this series.

```javascript
getTrendLines() : TrendlineCollection;
```


**Returns**

[TrendlineCollection](../trendlinecollection/)

### getSmooth() {#getSmooth--}

<b>@deprecated.</b> Please use the 'smooth' property instead. Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line and scatter connected by lines charts.

```javascript
getSmooth() : boolean;
```


### setSmooth(boolean) {#setSmooth-boolean-}

<b>@deprecated.</b> Please use the 'smooth' property instead. Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line and scatter connected by lines charts.

```javascript
setSmooth(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShadow() {#getShadow--}

<b>@deprecated.</b> Please use the 'shadow' property instead. True if the series has a shadow.

```javascript
getShadow() : boolean;
```


### setShadow(boolean) {#setShadow-boolean-}

<b>@deprecated.</b> Please use the 'shadow' property instead. True if the series has a shadow.

```javascript
setShadow(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHas3DEffect() {#getHas3DEffect--}

<b>@deprecated.</b> Please use the 'has3DEffect' property instead. True if the series has a three-dimensional appearance. Applies only to bubble charts.

```javascript
getHas3DEffect() : boolean;
```


### setHas3DEffect(boolean) {#setHas3DEffect-boolean-}

<b>@deprecated.</b> Please use the 'has3DEffect' property instead. True if the series has a three-dimensional appearance. Applies only to bubble charts.

```javascript
setHas3DEffect(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getBar3DShapeType() {#getBar3DShapeType--}

<b>@deprecated.</b> Please use the 'bar3DShapeType' property instead. Gets or sets the 3D shape type used with the 3-D bar or column chart.

```javascript
getBar3DShapeType() : Bar3DShapeType;
```


**Returns**

[Bar3DShapeType](../bar3dshapetype/)

### setBar3DShapeType(Bar3DShapeType) {#setBar3DShapeType-bar3dshapetype-}

<b>@deprecated.</b> Please use the 'bar3DShapeType' property instead. Gets or sets the 3D shape type used with the 3-D bar or column chart.

```javascript
setBar3DShapeType(value: Bar3DShapeType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Bar3DShapeType](../bar3dshapetype/) | The value to set. |

### getDataLabels() {#getDataLabels--}

<b>@deprecated.</b> Please use the 'dataLabels' property instead. Represents the DataLabels object for the specified ASeries.

```javascript
getDataLabels() : DataLabels;
```


**Returns**

[DataLabels](../datalabels/)

### getType() {#getType--}

<b>@deprecated.</b> Please use the 'type' property instead. Gets or sets a data series' type.

```javascript
getType() : ChartType;
```


**Returns**

[ChartType](../charttype/)

### setType(ChartType) {#setType-charttype-}

<b>@deprecated.</b> Please use the 'type' property instead. Gets or sets a data series' type.

```javascript
setType(value: ChartType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ChartType](../charttype/) | The value to set. |

### getMarker() {#getMarker--}

<b>@deprecated.</b> Please use the 'marker' property instead. Gets the <see cref="Marker">marker</see>.

```javascript
getMarker() : Marker;
```


**Returns**

[Marker](../marker/)

### getPlotOnSecondAxis() {#getPlotOnSecondAxis--}

<b>@deprecated.</b> Please use the 'plotOnSecondAxis' property instead. Indicates if this series is plotted on second value axis.

```javascript
getPlotOnSecondAxis() : boolean;
```


### setPlotOnSecondAxis(boolean) {#setPlotOnSecondAxis-boolean-}

<b>@deprecated.</b> Please use the 'plotOnSecondAxis' property instead. Indicates if this series is plotted on second value axis.

```javascript
setPlotOnSecondAxis(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getXErrorBar() {#getXErrorBar--}

<b>@deprecated.</b> Please use the 'xErrorBar' property instead. Represents X direction error bar of the series.

```javascript
getXErrorBar() : ErrorBar;
```


**Returns**

[ErrorBar](../errorbar/)

### getYErrorBar() {#getYErrorBar--}

<b>@deprecated.</b> Please use the 'yErrorBar' property instead. Represents Y direction error bar of the series.

```javascript
getYErrorBar() : ErrorBar;
```


**Returns**

[ErrorBar](../errorbar/)

### getHasHiLoLines() {#getHasHiLoLines--}

<b>@deprecated.</b> Please use the 'hasHiLoLines' property instead. True if the line chart has high-low lines. Applies only to line charts.

```javascript
getHasHiLoLines() : boolean;
```


### setHasHiLoLines(boolean) {#setHasHiLoLines-boolean-}

<b>@deprecated.</b> Please use the 'hasHiLoLines' property instead. True if the line chart has high-low lines. Applies only to line charts.

```javascript
setHasHiLoLines(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHiLoLines() {#getHiLoLines--}

<b>@deprecated.</b> Please use the 'hiLoLines' property instead. Returns a HiLoLines object that represents the high-low lines for a series on a line chart. Applies only to line charts.

```javascript
getHiLoLines() : Line;
```


**Returns**

[Line](../line/)

### getHasSeriesLines() {#getHasSeriesLines--}

<b>@deprecated.</b> Please use the 'hasSeriesLines' property instead. True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts.

```javascript
getHasSeriesLines() : boolean;
```


### setHasSeriesLines(boolean) {#setHasSeriesLines-boolean-}

<b>@deprecated.</b> Please use the 'hasSeriesLines' property instead. True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts.

```javascript
setHasSeriesLines(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSeriesLines() {#getSeriesLines--}

<b>@deprecated.</b> Please use the 'seriesLines' property instead. Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. Applies only to stacked bar and stacked column charts.

```javascript
getSeriesLines() : Line;
```


**Returns**

[Line](../line/)

### getHasDropLines() {#getHasDropLines--}

<b>@deprecated.</b> Please use the 'hasDropLines' property instead. True if the chart has drop lines. Applies only to line chart or area charts.

```javascript
getHasDropLines() : boolean;
```


### setHasDropLines(boolean) {#setHasDropLines-boolean-}

<b>@deprecated.</b> Please use the 'hasDropLines' property instead. True if the chart has drop lines. Applies only to line chart or area charts.

```javascript
setHasDropLines(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDropLines() {#getDropLines--}

<b>@deprecated.</b> Please use the 'dropLines' property instead. Returns a [Line](../line/) object that represents the drop lines for a series on the line chart or area chart. Applies only to line chart or area charts.

```javascript
getDropLines() : Line;
```


**Returns**

[Line](../line/)

### getHasUpDownBars() {#getHasUpDownBars--}

<b>@deprecated.</b> Please use the 'hasUpDownBars' property instead. True if a line chart has up and down bars. Applies only to line charts.

```javascript
getHasUpDownBars() : boolean;
```


### setHasUpDownBars(boolean) {#setHasUpDownBars-boolean-}

<b>@deprecated.</b> Please use the 'hasUpDownBars' property instead. True if a line chart has up and down bars. Applies only to line charts.

```javascript
setHasUpDownBars(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getUpBars() {#getUpBars--}

<b>@deprecated.</b> Please use the 'upBars' property instead. Returns an DropBars object that represents the up bars on a line chart. Applies only to line charts.

```javascript
getUpBars() : DropBars;
```


**Returns**

[DropBars](../dropbars/)

### getDownBars() {#getDownBars--}

<b>@deprecated.</b> Please use the 'downBars' property instead. Returns a [DropBars](../dropbars/) object that represents the down bars on a line chart. Applies only to line charts.

```javascript
getDownBars() : DropBars;
```


**Returns**

[DropBars](../dropbars/)

### isColorVaried() {#isColorVaried--}

<b>@deprecated.</b> Please use the 'isColorVaried' property instead. Represents if the color of points is varied. The chart must contain only one series.

```javascript
isColorVaried() : boolean;
```


### setIsColorVaried(boolean) {#setIsColorVaried-boolean-}

<b>@deprecated.</b> Please use the 'isColorVaried' property instead. Represents if the color of points is varied. The chart must contain only one series.

```javascript
setIsColorVaried(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getGapWidth() {#getGapWidth--}

<b>@deprecated.</b> Please use the 'gapWidth' property instead. Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500.

```javascript
getGapWidth() : number;
```


### setGapWidth(number) {#setGapWidth-number-}

<b>@deprecated.</b> Please use the 'gapWidth' property instead. Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500.

```javascript
setGapWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getFirstSliceAngle() {#getFirstSliceAngle--}

<b>@deprecated.</b> Please use the 'firstSliceAngle' property instead. Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.

```javascript
getFirstSliceAngle() : number;
```


### setFirstSliceAngle(number) {#setFirstSliceAngle-number-}

<b>@deprecated.</b> Please use the 'firstSliceAngle' property instead. Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.

```javascript
setFirstSliceAngle(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getOverlap() {#getOverlap--}

<b>@deprecated.</b> Please use the 'overlap' property instead. Specifies how bars and columns are positioned. Can be a value between – 100 and 100. Applies only to 2-D bar and 2-D column charts.

```javascript
getOverlap() : number;
```


### setOverlap(number) {#setOverlap-number-}

<b>@deprecated.</b> Please use the 'overlap' property instead. Specifies how bars and columns are positioned. Can be a value between – 100 and 100. Applies only to 2-D bar and 2-D column charts.

```javascript
setOverlap(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getSecondPlotSize() {#getSecondPlotSize--}

<b>@deprecated.</b> Please use the 'secondPlotSize' property instead. Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of the size of the primary pie. Can be a value from 5 to 200.

```javascript
getSecondPlotSize() : number;
```


### setSecondPlotSize(number) {#setSecondPlotSize-number-}

<b>@deprecated.</b> Please use the 'secondPlotSize' property instead. Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of the size of the primary pie. Can be a value from 5 to 200.

```javascript
setSecondPlotSize(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getSplitType() {#getSplitType--}

<b>@deprecated.</b> Please use the 'splitType' property instead. Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.

```javascript
getSplitType() : ChartSplitType;
```


**Returns**

[ChartSplitType](../chartsplittype/)

### setSplitType(ChartSplitType) {#setSplitType-chartsplittype-}

<b>@deprecated.</b> Please use the 'splitType' property instead. Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.

```javascript
setSplitType(value: ChartSplitType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ChartSplitType](../chartsplittype/) | The value to set. |

### getSplitValue() {#getSplitValue--}

<b>@deprecated.</b> Please use the 'splitValue' property instead. Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.

```javascript
getSplitValue() : number;
```


### setSplitValue(number) {#setSplitValue-number-}

<b>@deprecated.</b> Please use the 'splitValue' property instead. Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.

```javascript
setSplitValue(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isAutoSplit() {#isAutoSplit--}

<b>@deprecated.</b> Please use the 'isAutoSplit' property instead. Indicates whether the threshold value is automatic.

```javascript
isAutoSplit() : boolean;
```


### getBubbleScale() {#getBubbleScale--}

<b>@deprecated.</b> Please use the 'bubbleScale' property instead. Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, corresponding to a percentage of the default size. Applies only to bubble charts.

```javascript
getBubbleScale() : number;
```


### setBubbleScale(number) {#setBubbleScale-number-}

<b>@deprecated.</b> Please use the 'bubbleScale' property instead. Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, corresponding to a percentage of the default size. Applies only to bubble charts.

```javascript
setBubbleScale(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getSizeRepresents() {#getSizeRepresents--}

<b>@deprecated.</b> Please use the 'sizeRepresents' property instead. Gets or sets what the bubble size represents on a bubble chart.

```javascript
getSizeRepresents() : BubbleSizeRepresents;
```


**Returns**

[BubbleSizeRepresents](../bubblesizerepresents/)

**Remarks**

BubbleSizeRepresents.SizeIsArea means the value [Series.BubbleSizes](../series.bubblesizes/) is the area of the bubble. BubbleSizeRepresents.SizeIsWidth means the value [Series.BubbleSizes](../series.bubblesizes/) is the width of the bubble.

### setSizeRepresents(BubbleSizeRepresents) {#setSizeRepresents-bubblesizerepresents-}

<b>@deprecated.</b> Please use the 'sizeRepresents' property instead. Gets or sets what the bubble size represents on a bubble chart.

```javascript
setSizeRepresents(value: BubbleSizeRepresents) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [BubbleSizeRepresents](../bubblesizerepresents/) | The value to set. |

**Remarks**

BubbleSizeRepresents.SizeIsArea means the value [Series.BubbleSizes](../series.bubblesizes/) is the area of the bubble. BubbleSizeRepresents.SizeIsWidth means the value [Series.BubbleSizes](../series.bubblesizes/) is the width of the bubble.

### getShowNegativeBubbles() {#getShowNegativeBubbles--}

<b>@deprecated.</b> Please use the 'showNegativeBubbles' property instead. True if negative bubbles are shown for the chart group. Valid only for bubble charts.

```javascript
getShowNegativeBubbles() : boolean;
```


### setShowNegativeBubbles(boolean) {#setShowNegativeBubbles-boolean-}

<b>@deprecated.</b> Please use the 'showNegativeBubbles' property instead. True if negative bubbles are shown for the chart group. Valid only for bubble charts.

```javascript
setShowNegativeBubbles(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDoughnutHoleSize() {#getDoughnutHoleSize--}

<b>@deprecated.</b> Please use the 'doughnutHoleSize' property instead. Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart size, between 10 and 90 percent.

```javascript
getDoughnutHoleSize() : number;
```


### setDoughnutHoleSize(number) {#setDoughnutHoleSize-number-}

<b>@deprecated.</b> Please use the 'doughnutHoleSize' property instead. Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart size, between 10 and 90 percent.

```javascript
setDoughnutHoleSize(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getExplosion() {#getExplosion--}

<b>@deprecated.</b> Please use the 'explosion' property instead. The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.

```javascript
getExplosion() : number;
```


### setExplosion(number) {#setExplosion-number-}

<b>@deprecated.</b> Please use the 'explosion' property instead. The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.

```javascript
setExplosion(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHasRadarAxisLabels() {#getHasRadarAxisLabels--}

<b>@deprecated.</b> Please use the 'hasRadarAxisLabels' property instead. True if a radar chart has category axis labels. Applies only to radar charts.

```javascript
getHasRadarAxisLabels() : boolean;
```


### setHasRadarAxisLabels(boolean) {#setHasRadarAxisLabels-boolean-}

<b>@deprecated.</b> Please use the 'hasRadarAxisLabels' property instead. True if a radar chart has category axis labels. Applies only to radar charts.

```javascript
setHasRadarAxisLabels(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHasLeaderLines() {#getHasLeaderLines--}

<b>@deprecated.</b> Please use the 'hasLeaderLines' property instead. True if the series has leader lines.

```javascript
getHasLeaderLines() : boolean;
```


### setHasLeaderLines(boolean) {#setHasLeaderLines-boolean-}

<b>@deprecated.</b> Please use the 'hasLeaderLines' property instead. True if the series has leader lines.

```javascript
setHasLeaderLines(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getLeaderLines() {#getLeaderLines--}

<b>@deprecated.</b> Please use the 'leaderLines' property instead. Represents leader lines on a chart. Leader lines connect data labels to data points. This object isn’t a collection; there’s no object that represents a single leader line.

```javascript
getLeaderLines() : Line;
```


**Returns**

[Line](../line/)

### getLegendEntry() {#getLegendEntry--}

<b>@deprecated.</b> Please use the 'legendEntry' property instead. Gets the legend entry according to this series.

```javascript
getLegendEntry() : LegendEntry;
```


**Returns**

[LegendEntry](../legendentry/)

### getShapeProperties() {#getShapeProperties--}

<b>@deprecated.</b> Please use the 'shapeProperties' property instead. Gets the [ShapePropertyCollection](../shapepropertycollection/) object that holds the visual shape properties of the Series.

```javascript
getShapeProperties() : ShapePropertyCollection;
```


**Returns**

[ShapePropertyCollection](../shapepropertycollection/)

### move(number) {#move-number-}

Moves the series up or down.

```javascript
move(count: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| count | number | The number of moving up or down.         /// Move the series up if this is less than zero;         /// Move the series down if this is greater than zero. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



