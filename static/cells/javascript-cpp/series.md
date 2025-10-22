##Series
Encapsulates the object that represents a single data series in a chart.
## Series class
Encapsulates the object that represents a single data series in a chart.
```javascript
class Series;
```
### Example
```javascript
const { Workbook, ChartType, ChartMarkerType, FormattingType, Color, SaveFormat } = AsposeCells;
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
var uint8Array = workbook.save(SaveFormat.Xlsx);
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
| [move(number)](#move-number-)| Moves the series up or down. |
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
const { Workbook, ChartType } = AsposeCells;
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
### move(number) {#move-number-}
Moves the series up or down.
```javascript
move(count: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| count | number | The number of moving up or down.         /// Move the series up if this is less than zero;         /// Move the series down if this is greater than zero. |
