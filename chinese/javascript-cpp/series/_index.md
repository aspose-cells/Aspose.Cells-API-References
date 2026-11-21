---
title: Series
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates the object that represents a single data series in a chart.
type: docs
url: /zh/javascript-cpp/series/
---

## Series class

Encapsulates the object that represents a single data series in a chart.

```javascript
class Series;
```


### Example
```javascript
const { Workbook, ChartType, ChartMarkerType, FormattingType, Color, SaveFormat } = AsposeCells;

//实例化一个 Workbook 对象
var workbook = new Workbook();
//向 Excel 对象添加新工作表
var sheetIndex = workbook.worksheets.add();
//通过传递工作表索引获取新添加工作表的引用
var worksheet = workbook.worksheets.get(sheetIndex);
//向 "A1" 单元格添加示例值
worksheet.cells.get("A1").putValue(50);
//向 "A2" 单元格添加示例值
worksheet.cells.get("A2").putValue(100);
//向 "A3" 单元格添加示例值
worksheet.cells.get("A3").putValue(150);
//向 "A4" 单元格添加示例值
worksheet.cells.get("A4").putValue(200);
//向 "B1" 单元格添加示例值
worksheet.cells.get("B1").putValue(60);
//向 "B2" 单元格添加示例值
worksheet.cells.get("B2").putValue(32);
//向 "B3" 单元格添加示例值
worksheet.cells.get("B3").putValue(50);
//向 "B4" 单元格添加示例值
worksheet.cells.get("B4").putValue(40);
//向 "C1" 单元格添加示例值作为类别数据
worksheet.cells.get("C1").putValue("Q1");
//向 "C2" 单元格添加示例值作为类别数据
worksheet.cells.get("C2").putValue("Q2");
//将示例值添加到 "C3" 单元格作为类别数据
worksheet.cells.get("C3").putValue("Y1");
//将示例值添加到 "C4" 单元格作为类别数据
worksheet.cells.get("C4").putValue("Y2");
//向工作表添加图表
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//访问新添加图表的实例
var chart = worksheet.charts.get(chartIndex);
//向图表添加 NSeries（图表数据源），范围从 "A1" 单元格到 "B4"
chart.nSeries.add("A1:B4", true);
//设置 NSeries 类别数据的数据源
chart.nSeries.categoryData = "C1:C4";
var series = chart.nSeries.get(1);
//设置系列的值。
series.values = "=B1:B4";
//更改系列的图表类型。
series.type = ChartType.Line;
//设置标记属性。
series.marker.markerStyle = ChartMarkerType.Circle;
series.marker.foregroundColorSetType = FormattingType.Automatic;
series.marker.foregroundColor = Color.Black;
series.marker.backgroundColorSetType = FormattingType.Automatic;
//保存 Excel 文件
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Properties

| Property | Type | Description |
| --- | --- | --- |
| [isFiltered](#isFiltered--)| boolean | Indicates whether the series is selected or filtered. True indicates that this series is filtered, and it will not be displayed on the chart. |
| [layoutProperties](#layoutProperties--)| SeriesLayoutProperties | Readonly. Represents the properties of layout. |
| [points](#points--)| ChartPointCollection | Readonly. Gets the collection of points in a series in a chart. |
| [area](#area--)| Area | Readonly. Represents the background area of the Series object. |
| [border](#border--)| Line | Readonly. Represents the border of a Series object. |
| [name](#name--)| string | Gets or sets the name of the data series. |
| [displayName](#displayName--)| string | Readonly. Gets the series's name that displays on the chart graph. |
| [countOfDataValues](#countOfDataValues--)| number | Readonly. Gets the number of the data values. |
| [isVerticalValues](#isVerticalValues--)| boolean | Readonly. Indicates whether the data source is vertical. |
| [values](#values--)| string | Represents the Y values of this chart series. |
| [pointValues](#pointValues--)| ChartDataValue[] | Readonly. Gets the actual values that are used to plot every point of this series in the chart. |
| [categoryValues](#categoryValues--)| ChartDataValue[][] | Readonly. Gets the actual category values that are used to plot every point of this series in the chart. |
| [valuesFormatCode](#valuesFormatCode--)| string | Represents the format code of the Values NumberList. |
| [xValuesFormatCode](#xValuesFormatCode--)| string | Represents format code of X Values' NumberList. |
| [xValues](#xValues--)| string | Represents the X values of this chart series. |
| [bubbleSizes](#bubbleSizes--)| string | Gets or sets the bubble size values of the chart series. |
| [trendLines](#trendLines--)| TrendlineCollection | Readonly. Returns all the trendlines of this series. |
| [smooth](#smooth--)| boolean | Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line charts and scatter charts with lines. |
| [shadow](#shadow--)| boolean | True if the series has a shadow. |
| [has3DEffect](#has3DEffect--)| boolean | True if the series has a three-dimensional appearance. |
| [bar3DShapeType](#bar3DShapeType--)| Bar3DShapeType | Gets or sets the 3D shape type used with the 3-D bar or column chart. |
| [dataLabels](#dataLabels--)| DataLabels | Readonly. Represents the DataLabels object for the specified ASeries. |
| [type](#type--)| ChartType | Gets or sets a data series' type. |
| [marker](#marker--)| Marker | Readonly. Gets the <see cref="Marker">marker</see>. |
| [plotOnSecondAxis](#plotOnSecondAxis--)| boolean | Indicates if this series is plotted on the second value axis. |
| [xErrorBar](#xErrorBar--)| ErrorBar | Readonly. Represents X direction error bar of the series. |
| [yErrorBar](#yErrorBar--)| ErrorBar | Readonly. Represents Y direction error bar of the series. |
| [hasHiLoLines](#hasHiLoLines--)| boolean | True if the line chart has high-low lines. Applies only to line charts. |
| [hiLoLines](#hiLoLines--)| Line | Readonly. Returns a HiLoLines object that represents the high-low lines for a series on a line chart. Applies only to line charts. |
| [hasSeriesLines](#hasSeriesLines--)| boolean | True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts. |
| [seriesLines](#seriesLines--)| Line | Readonly. Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. Applies only to stacked bar and stacked column charts. |
| [hasDropLines](#hasDropLines--)| boolean | True if the chart has drop lines. Applies only to line chart or area charts. |
| [dropLines](#dropLines--)| Line | Readonly. Returns a [Line](../line/) object that represents the drop lines for a series on the line chart or area chart. Applies only to line charts or area charts. |
| [hasUpDownBars](#hasUpDownBars--)| boolean | True if a line chart has up and down bars. Applies only to line charts. |
| [upBars](#upBars--)| DropBars | Readonly. Returns a DropBars object that represents the up bars on a line chart. Applies only to line charts. |
| [downBars](#downBars--)| DropBars | Readonly. Returns a [DropBars](../dropbars/) object that represents the down bars on a line chart. Applies only to line charts. |
| [isColorVaried](#isColorVaried--)| boolean | Represents whether the color of points is varied. The chart must contain only one series or this chart is a pie chart. |
| [gapWidth](#gapWidth--)| number | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500. |
| [firstSliceAngle](#firstSliceAngle--)| number | Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, with values from 0 to 360. |
| [overlap](#overlap--)| number | Specifies how bars and columns are positioned. Can be a value between -100 and 100. Applies only to 2-D bar and 2-D column charts. |
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
| [leaderLines](#leaderLines--)| Line | Readonly. Represents leader lines on a chart. Leader lines connect data labels to data points. This object isn't a collection; there's no object that represents a single leader line. |
| [legendEntry](#legendEntry--)| LegendEntry | Readonly. Gets the legend entry according to this series. |
| [shapeProperties](#shapeProperties--)| ShapePropertyCollection | Readonly. Gets the [ShapePropertyCollection](../shapepropertycollection/) object that holds the visual shape properties of the Series. |

## Methods

| Method | Description |
| --- | --- |
| [move(number)](#move-number-)| Moves the series up or down. |


### isFiltered {#isFiltered--}

Indicates whether the series is selected or filtered. True indicates that this series is filtered, and it will not be displayed on the chart.

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

Readonly. Represents the background area of the Series object.

```javascript
area : Area;
```


### border {#border--}

Readonly. Represents the border of a Series object.

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
const { Workbook, ChartType } = AsposeCells;

var workbook = new Workbook();
//获取第一个工作表。
var worksheet = workbook.worksheets.get(0);
//向工作表添加图表
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//访问新添加图表的实例
var chart = worksheet.charts.get(chartIndex);
//向图表添加 NSeries（图表数据源），范围从 "A1" 单元格到 "B4"
chart.nSeries.add("A1:B4", true);
//引用单元格的名称
chart.nSeries.get(0).name = "=A1";
//将字符串设置为名称
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


**Remarks**

To get the actual values(corresponding to every point of this series) defined by this property, please use [PointValues](../pointvalues/).

### pointValues {#pointValues--}

Readonly. Gets the actual values that are used to plot every point of this series in the chart.

```javascript
pointValues : ChartDataValue[];
```


**Remarks**

This property provides one convenient way to get the actual values corresponding to the data defined by [Series.Values](../series.values/), especially when the specified data source is external link, formula, ...etc.

### categoryValues {#categoryValues--}

Readonly. Gets the actual category values that are used to plot every point of this series in the chart.

```javascript
categoryValues : ChartDataValue[][];
```


**Remarks**

This property provides one convenient way to get the actual values corresponding to the data defined by [Series.XValues](../series.xvalues/), especially when the specified data source is external link, formula, ...etc.

### valuesFormatCode {#valuesFormatCode--}

Represents the format code of the Values NumberList.

```javascript
valuesFormatCode : string;
```


### xValuesFormatCode {#xValuesFormatCode--}

Represents format code of X Values' NumberList.

```javascript
xValuesFormatCode : string;
```


### xValues {#xValues--}

Represents the X values of this chart series.

```javascript
xValues : string;
```


**Remarks**

Only for Scatter and Bubble chart. Please use [SeriesCollection.CategoryData](../seriescollection.categorydata/) for other types of charts [CategoryValues](../categoryvalues/) is used to get the actual category values of this series.

### bubbleSizes {#bubbleSizes--}

Gets or sets the bubble size values of the chart series.

```javascript
bubbleSizes : string;
```


**Remarks**

Only for [ChartType.Bubble](../charttype.bubble/) or [ChartType.Bubble3D](../charttype.bubble3d/).

### trendLines {#trendLines--}

Readonly. Returns all the trendlines of this series.

```javascript
trendLines : TrendlineCollection;
```


### smooth {#smooth--}

Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line charts and scatter charts with lines.

```javascript
smooth : boolean;
```


### shadow {#shadow--}

True if the series has a shadow.

```javascript
shadow : boolean;
```


### has3DEffect {#has3DEffect--}

True if the series has a three-dimensional appearance.

```javascript
has3DEffect : boolean;
```


**Remarks**

Applies only to [ChartType.Bubble](../charttype.bubble/) or [ChartType.Bubble3D](../charttype.bubble3d/) charts.

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

Indicates if this series is plotted on the second value axis.

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

Readonly. Returns a [Line](../line/) object that represents the drop lines for a series on the line chart or area chart. Applies only to line charts or area charts.

```javascript
dropLines : Line;
```


### hasUpDownBars {#hasUpDownBars--}

True if a line chart has up and down bars. Applies only to line charts.

```javascript
hasUpDownBars : boolean;
```


### upBars {#upBars--}

Readonly. Returns a DropBars object that represents the up bars on a line chart. Applies only to line charts.

```javascript
upBars : DropBars;
```


### downBars {#downBars--}

Readonly. Returns a [DropBars](../dropbars/) object that represents the down bars on a line chart. Applies only to line charts.

```javascript
downBars : DropBars;
```


### isColorVaried {#isColorVaried--}

Represents whether the color of points is varied. The chart must contain only one series or this chart is a pie chart.

```javascript
isColorVaried : boolean;
```


### gapWidth {#gapWidth--}

Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500.

```javascript
gapWidth : number;
```


### firstSliceAngle {#firstSliceAngle--}

Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, with values from 0 to 360.

```javascript
firstSliceAngle : number;
```


### overlap {#overlap--}

Specifies how bars and columns are positioned. Can be a value between -100 and 100. Applies only to 2-D bar and 2-D column charts.

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

Readonly. Represents leader lines on a chart. Leader lines connect data labels to data points. This object isn't a collection; there's no object that represents a single leader line.

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


### move(number) {#move-number-}

Moves the series up or down.

```javascript
move(count: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| count | number | The number of moving up or down.         /// Move the series up if this is less than zero;         /// Move the series down if this is greater than zero. |


