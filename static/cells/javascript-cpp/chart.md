##Chart
Encapsulates the object that represents a single Excel chart.
## Chart class
Encapsulates the object that represents a single Excel chart.
```javascript
class Chart;
```
### Example
```javascript
const { Workbook, ChartType } = AsposeCells;
var workbook = new Workbook();
var sheet = workbook.worksheets.get(0);
var cells = sheet.cells;
cells.get(0, 1).putValue("Income");
cells.get(1, 0).putValue("Company A");
cells.get(2, 0).putValue("Company B");
cells.get(3, 0).putValue("Company C");
cells.get(1, 1).putValue(10000);
cells.get(2, 1).putValue(20000);
cells.get(3, 1).putValue(30000);
var chartIndex = sheet.charts.add(ChartType.Column, 9, 9, 21, 15);
var chart = sheet.charts.get(chartIndex);
chart.nSeries.add("B2:B4", true);
chart.nSeries.categoryData = "A2:A4";
var aSeries = chart.nSeries.get(0);
aSeries.name = "=B1";
chart.showLegend = true;
chart.title.text = "Income Analysis";
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [style](#style--)| number | Gets and sets the builtin style. |
| [chartObject](#chartObject--)| ChartShape | Readonly. Represents the chartShape; |
| [hidePivotFieldButtons](#hidePivotFieldButtons--)| boolean | Indicates whether hide the pivot chart field buttons only when the chart is PivotChart. |
| [pivotOptions](#pivotOptions--)| PivotOptions | Readonly. Specifies the pivot controls that appear on the chart |
| [pivotSource](#pivotSource--)| string | The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart. |
| [plotBy](#plotBy--)| PlotDataByType | Readonly. Gets and sets whether plot by row or column. |
| [plotEmptyCellsType](#plotEmptyCellsType--)| PlotEmptyCellsType | Gets and sets  how to plot the empty cells. |
| [plotVisibleCellsOnly](#plotVisibleCellsOnly--)| boolean | Indicates whether plot visible cells only. |
| [displayNaAsBlank](#displayNaAsBlank--)| boolean | Indicates whether displaying #N/A as blank value. |
| [name](#name--)| string | Gets and sets the name of the chart. |
| [sizeWithWindow](#sizeWithWindow--)| boolean | True if Microsoft Excel resizes the chart to match the size of the chart sheet window. |
| [worksheet](#worksheet--)| Worksheet | Readonly. Gets the worksheet which contains this chart. |
| [shapes](#shapes--)| ShapeCollection | Readonly. Returns all drawing shapes in this chart. |
| [printSize](#printSize--)| PrintSizeType | Gets and sets the printed chart size. |
| [type](#type--)| ChartType | Gets or sets a chart's type. |
| [nSeries](#nSeries--)| SeriesCollection | Readonly. Gets a [SeriesCollection](../seriescollection/) collection representing the data series in the chart. |
| [filteredNSeries](#filteredNSeries--)| SeriesCollection | Readonly. Gets a [SeriesCollection](../seriescollection/) collection representing the data series that are filtered in the chart. |
| [title](#title--)| Title | Readonly. Gets the chart's title. |
| [subTitle](#subTitle--)| Title | Readonly. Gets the chart's sub-title. Only for ODS format file. |
| [plotArea](#plotArea--)| PlotArea | Readonly. Gets the chart's plot area which includes axis tick labels. |
| [chartArea](#chartArea--)| ChartArea | Readonly. Gets the chart area in the worksheet. |
| [categoryAxis](#categoryAxis--)| Axis | Readonly. Gets the chart's X axis. |
| [valueAxis](#valueAxis--)| Axis | Readonly. Gets the chart's Y axis. |
| [secondValueAxis](#secondValueAxis--)| Axis | Readonly. Gets the chart's second Y axis. |
| [secondCategoryAxis](#secondCategoryAxis--)| Axis | Readonly. Gets the chart's second X axis. |
| [seriesAxis](#seriesAxis--)| Axis | Readonly. Gets the chart's series axis. |
| [legend](#legend--)| Legend | Readonly. Gets the chart legend. |
| [chartDataTable](#chartDataTable--)| ChartDataTable | Readonly. Represents the chart data table. |
| [showLegend](#showLegend--)| boolean | Gets or sets a value indicating whether the chart legend will be displayed. Default is true. |
| [isRectangularCornered](#isRectangularCornered--)| boolean | Gets or sets a value indicating whether the chart area is rectangular cornered. Default is true. |
| [showDataTable](#showDataTable--)| boolean | Gets or sets a value indicating whether the chart displays a data table. |
| [firstSliceAngle](#firstSliceAngle--)| number | Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360. |
| [gapWidth](#gapWidth--)| number | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500. |
| [gapDepth](#gapDepth--)| number | Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width. The value of this property must be between 0 and 500. |
| [floor](#floor--)| Floor | Readonly. Returns a [Floor](../floor/) object that represents the walls of a 3-D chart. |
| [walls](#walls--)| Walls | Readonly. Returns a [Walls](../walls/) object that represents the walls of a 3-D chart. |
| [backWall](#backWall--)| Walls | Readonly. Returns a [Walls](../walls/) object that represents the back wall of a 3-D chart. |
| [sideWall](#sideWall--)| Walls | Readonly. Returns a [Walls](../walls/) object that represents the side wall of a 3-D chart. |
| [wallsAndGridlines2D](#wallsAndGridlines2D--)| boolean | True if gridlines are drawn two-dimensionally on a 3-D chart. |
| [rotationAngle](#rotationAngle--)| number | Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees). |
| [elevation](#elevation--)| number | Represents the elevation of the 3-D chart view, in degrees. |
| [rightAngleAxes](#rightAngleAxes--)| boolean | True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie Charts). |
| [autoScaling](#autoScaling--)| boolean | True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. The RightAngleAxes property must be True. |
| [heightPercent](#heightPercent--)| number | Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent). |
| [perspective](#perspective--)| number | Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100. This property is ignored if the RightAngleAxes property is True. |
| [is3D](#is3D--)| boolean | Readonly. Indicates whether the chart is a 3d chart. |
| [depthPercent](#depthPercent--)| number | Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent). |
| [placement](#placement--)| PlacementType | Represents the way the chart is attached to the cells below it. |
| [pageSetup](#pageSetup--)| PageSetup | Readonly. Represents the page setup description in this chart. |
| [line](#line--)| Line | Readonly. Gets the line. |
## Methods
| Method | Description |
| --- | --- |
| [isCellReferedByChart(number, number, number)](#isCellReferedByChart-number-number-number-)| Returns whether the cell refered by the chart. |
| [isChartDataChanged()](#isChartDataChanged--)| Detects if a chart's data source has changed. |
| [refreshPivotData()](#refreshPivotData--)| Refreshes chart's data from pivot table. |
| [changeTemplate(Uint8Array)](#changeTemplate-uint8array-)| Change chart type with preset template. |
| [move(number, number, number, number)](#move-number-number-number-number-)| Moves the chart to a specified location. |
| [calculate()](#calculate--)| Calculates the custom position of plot area, axes if the position of them are auto assigned. |
| [calculate(ChartCalculateOptions)](#calculate-chartcalculateoptions-)| Calculates the custom position of plot area, axes if the position of them are auto assigned, with Chart Calculate Options. |
| [toImageAsync(string)](#toImageAsync-string-)| Creates the chart image and saves it to a file. The extension of the file name determines the format of the image. |
| [toImageAsync(string, ImageType)](#toImageAsync-string-imagetype-)| Creates the chart image and saves it to a file in the specified image type. |
| [toImageAsync(string, number)](#toImageAsync-string-number-)| Creates the chart image and saves it to a file in the Jpeg format. |
| [toImageAsync(number)](#toImageAsync-number-)| Creates the chart image and saves it to a stream in the Jpeg format. |
| [toImageAsync(ImageType)](#toImageAsync-imagetype-)| Creates the chart image and saves it to a stream in the specified format. |
| [toImageAsync(string, ImageOrPrintOptions)](#toImageAsync-string-imageorprintoptions-)| Creates the chart image and saves it to a file. The extension of the file name determines the format of the image. |
| [toImageAsync(ImageOrPrintOptions)](#toImageAsync-imageorprintoptions-)| Creates the chart image and saves it to a stream in the specified format. |
| [toImage(string)](#toImage-string-)| Creates the chart image and saves it to a file. The extension of the file name determines the format of the image. |
| [toImage(string, ImageType)](#toImage-string-imagetype-)| Creates the chart image and saves it to a file in the specified image type. |
| [toImage(string, number)](#toImage-string-number-)| Creates the chart image and saves it to a file in the Jpeg format. |
| [toImage(number)](#toImage-number-)| Creates the chart image and saves it to a stream in the Jpeg format. |
| [toImage(ImageType)](#toImage-imagetype-)| Creates the chart image and saves it to a stream in the specified format. |
| [toImage(string, ImageOrPrintOptions)](#toImage-string-imageorprintoptions-)| Creates the chart image and saves it to a file. The extension of the file name determines the format of the image. |
| [toImage(ImageOrPrintOptions)](#toImage-imageorprintoptions-)| Creates the chart image and saves it to a stream in the specified format. |
| [toPdfAsync(string)](#toPdfAsync-string-)| Saves the chart to a pdf file. |
| [toPdfAsync(string, number, number, PageLayoutAlignmentType, PageLayoutAlignmentType)](#toPdfAsync-string-number-number-pagelayoutalignmenttype-pagelayoutalignmenttype-)| Saves the chart to a pdf file. |
| [toPdfAsync()](#toPdfAsync--)| Creates the chart pdf and saves it to a stream. |
| [toPdfAsync(number, number, PageLayoutAlignmentType, PageLayoutAlignmentType)](#toPdfAsync-number-number-pagelayoutalignmenttype-pagelayoutalignmenttype-)| Creates the chart pdf and saves it to a stream. |
| [toPdf(string)](#toPdf-string-)| Saves the chart to a pdf file. |
| [toPdf(string, number, number, PageLayoutAlignmentType, PageLayoutAlignmentType)](#toPdf-string-number-number-pagelayoutalignmenttype-pagelayoutalignmenttype-)| Saves the chart to a pdf file. |
| [toPdf()](#toPdf--)| Creates the chart pdf and saves it to a stream. |
| [toPdf(number, number, PageLayoutAlignmentType, PageLayoutAlignmentType)](#toPdf-number-number-pagelayoutalignmenttype-pagelayoutalignmenttype-)| Creates the chart pdf and saves it to a stream. |
| [getActualSize()](#getActualSize--)| Gets actual size of chart in unit of pixels. |
| [hasAxis(AxisType, boolean)](#hasAxis-axistype-boolean-)| Returns which axes exist on the chart. |
| [switchRowColumn()](#switchRowColumn--)| Switches row/column. |
| [getChartDataRange()](#getChartDataRange--)| Gets the data source range of the chart. |
| [setChartDataRange(string, boolean)](#setChartDataRange-string-boolean-)| Specifies data range for a chart. |
### style {#style--}
Gets and sets the builtin style.
```javascript
style : number;
```
**Remarks**
It should be between 1 and 48. Return -1 if it's not be set.
### chartObject {#chartObject--}
Readonly. Represents the chartShape;
```javascript
chartObject : ChartShape;
```
### hidePivotFieldButtons {#hidePivotFieldButtons--}
Indicates whether hide the pivot chart field buttons only when the chart is PivotChart.
```javascript
hidePivotFieldButtons : boolean;
```
### pivotOptions {#pivotOptions--}
Readonly. Specifies the pivot controls that appear on the chart
```javascript
pivotOptions : PivotOptions;
```
### pivotSource {#pivotSource--}
The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart.
```javascript
pivotSource : string;
```
**Remarks**
If the pivot table  "PivotTable1" in the Worksheet "Sheet1" in the file "Book1.xls". The pivotSource could be "[Book1.xls]Sheet1!PivotTable1" if the chart and the PivotTable is not in the same workbook. If you set this property ,the previous data source setting will be lost.
### plotBy {#plotBy--}
Readonly. Gets and sets whether plot by row or column.
```javascript
plotBy : PlotDataByType;
```
### plotEmptyCellsType {#plotEmptyCellsType--}
Gets and sets  how to plot the empty cells.
```javascript
plotEmptyCellsType : PlotEmptyCellsType;
```
### plotVisibleCellsOnly {#plotVisibleCellsOnly--}
Indicates whether plot visible cells only.
```javascript
plotVisibleCellsOnly : boolean;
```
### displayNaAsBlank {#displayNaAsBlank--}
Indicates whether displaying #N/A as blank value.
```javascript
displayNaAsBlank : boolean;
```
### name {#name--}
Gets and sets the name of the chart.
```javascript
name : string;
```
### sizeWithWindow {#sizeWithWindow--}
True if Microsoft Excel resizes the chart to match the size of the chart sheet window.
```javascript
sizeWithWindow : boolean;
```
### worksheet {#worksheet--}
Readonly. Gets the worksheet which contains this chart.
```javascript
worksheet : Worksheet;
```
### shapes {#shapes--}
Readonly. Returns all drawing shapes in this chart.
```javascript
shapes : ShapeCollection;
```
### printSize {#printSize--}
Gets and sets the printed chart size.
```javascript
printSize : PrintSizeType;
```
### type {#type--}
Gets or sets a chart's type.
```javascript
type : ChartType;
```
### nSeries {#nSeries--}
Readonly. Gets a [SeriesCollection](../seriescollection/) collection representing the data series in the chart.
```javascript
nSeries : SeriesCollection;
```
### filteredNSeries {#filteredNSeries--}
Readonly. Gets a [SeriesCollection](../seriescollection/) collection representing the data series that are filtered in the chart.
```javascript
filteredNSeries : SeriesCollection;
```
### title {#title--}
Readonly. Gets the chart's title.
```javascript
title : Title;
```
### subTitle {#subTitle--}
Readonly. Gets the chart's sub-title. Only for ODS format file.
```javascript
subTitle : Title;
```
### plotArea {#plotArea--}
Readonly. Gets the chart's plot area which includes axis tick labels.
```javascript
plotArea : PlotArea;
```
### chartArea {#chartArea--}
Readonly. Gets the chart area in the worksheet.
```javascript
chartArea : ChartArea;
```
### categoryAxis {#categoryAxis--}
Readonly. Gets the chart's X axis.
```javascript
categoryAxis : Axis;
```
### valueAxis {#valueAxis--}
Readonly. Gets the chart's Y axis.
```javascript
valueAxis : Axis;
```
### secondValueAxis {#secondValueAxis--}
Readonly. Gets the chart's second Y axis.
```javascript
secondValueAxis : Axis;
```
### secondCategoryAxis {#secondCategoryAxis--}
Readonly. Gets the chart's second X axis.
```javascript
secondCategoryAxis : Axis;
```
### seriesAxis {#seriesAxis--}
Readonly. Gets the chart's series axis.
```javascript
seriesAxis : Axis;
```
### legend {#legend--}
Readonly. Gets the chart legend.
```javascript
legend : Legend;
```
### chartDataTable {#chartDataTable--}
Readonly. Represents the chart data table.
```javascript
chartDataTable : ChartDataTable;
```
### showLegend {#showLegend--}
Gets or sets a value indicating whether the chart legend will be displayed. Default is true.
```javascript
showLegend : boolean;
```
### isRectangularCornered {#isRectangularCornered--}
Gets or sets a value indicating whether the chart area is rectangular cornered. Default is true.
```javascript
isRectangularCornered : boolean;
```
### showDataTable {#showDataTable--}
Gets or sets a value indicating whether the chart displays a data table.
```javascript
showDataTable : boolean;
```
### firstSliceAngle {#firstSliceAngle--}
Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.
```javascript
firstSliceAngle : number;
```
### gapWidth {#gapWidth--}
Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500.
```javascript
gapWidth : number;
```
### gapDepth {#gapDepth--}
Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width. The value of this property must be between 0 and 500.
```javascript
gapDepth : number;
```
### floor {#floor--}
Readonly. Returns a [Floor](../floor/) object that represents the walls of a 3-D chart.
```javascript
floor : Floor;
```
**Remarks**
This property doesn't apply to 3-D pie charts.
### walls {#walls--}
Readonly. Returns a [Walls](../walls/) object that represents the walls of a 3-D chart.
```javascript
walls : Walls;
```
**Remarks**
This property doesn't apply to 3-D pie charts.
### backWall {#backWall--}
Readonly. Returns a [Walls](../walls/) object that represents the back wall of a 3-D chart.
```javascript
backWall : Walls;
```
### sideWall {#sideWall--}
Readonly. Returns a [Walls](../walls/) object that represents the side wall of a 3-D chart.
```javascript
sideWall : Walls;
```
### wallsAndGridlines2D {#wallsAndGridlines2D--}
True if gridlines are drawn two-dimensionally on a 3-D chart.
```javascript
wallsAndGridlines2D : boolean;
```
### rotationAngle {#rotationAngle--}
Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees).
```javascript
rotationAngle : number;
```
**Remarks**
The value of this property must be from 0 to 360, except for 3-D bar charts, where the value must be from 0 to 44. The default value is 20. Applies only to 3-D charts.
### elevation {#elevation--}
Represents the elevation of the 3-D chart view, in degrees.
```javascript
elevation : number;
```
**Remarks**
The chart elevation is the height at which you view the chart, in degrees. The default is 15 for most chart types. The value of this property must be between -90 and 90, except for 3-D bar charts, where it must be between 0 and 44.
### rightAngleAxes {#rightAngleAxes--}
True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie Charts).
```javascript
rightAngleAxes : boolean;
```
**Remarks**
If this property is True, the Perspective property is ignored.
### autoScaling {#autoScaling--}
True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. The RightAngleAxes property must be True.
```javascript
autoScaling : boolean;
```
### heightPercent {#heightPercent--}
Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent).
```javascript
heightPercent : number;
```
### perspective {#perspective--}
Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100. This property is ignored if the RightAngleAxes property is True.
```javascript
perspective : number;
```
### is3D {#is3D--}
Readonly. Indicates whether the chart is a 3d chart.
```javascript
is3D : boolean;
```
### depthPercent {#depthPercent--}
Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent).
```javascript
depthPercent : number;
```
### placement {#placement--}
Represents the way the chart is attached to the cells below it.
```javascript
placement : PlacementType;
```
### pageSetup {#pageSetup--}
Readonly. Represents the page setup description in this chart.
```javascript
pageSetup : PageSetup;
```
### line {#line--}
Readonly. Gets the line.
```javascript
line : Line;
```
### isCellReferedByChart(number, number, number) {#isCellReferedByChart-number-number-number-}
Returns whether the cell refered by the chart.
```javascript
isCellReferedByChart(sheetIndex: number, rowIndex: number, columnIndex: number) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | number | The sheet Index.-1 means the worksheet which contains current chart. |
| rowIndex | number | The row index |
| columnIndex | number | The column index |
### isChartDataChanged() {#isChartDataChanged--}
Detects if a chart's data source has changed.
```javascript
isChartDataChanged() : boolean;
```
**Returns**
Returns true if the chart has changed otherwise returns false
**Remarks**
The method detects the changes in the chart's data source before rendering the chart to image format. At first Chart.toImage call, the chart source data (e.g. XValuesParseData, ValuesParseData) will be recorded. Before calling the Chart.toImage method again, call IsChartDataChanged method to check if Chart needs re-rendering.
### refreshPivotData() {#refreshPivotData--}
Refreshes chart's data from pivot table.
```javascript
refreshPivotData() : void;
```
**Remarks**
We will gather data from pivot data source to the pivot table report. This method is only used to gather all data to a pivot chart.
### changeTemplate(Uint8Array) {#changeTemplate-uint8array-}
Change chart type with preset template.
```javascript
changeTemplate(data: Uint8Array) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| data | number[] | The data of chart template file(.crtx). |
### move(number, number, number, number) {#move-number-number-number-number-}
Moves the chart to a specified location.
```javascript
move(upperLeftRow: number, upperLeftColumn: number, lowerRightRow: number, lowerRightColumn: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| upperLeftColumn | number | Upper left column index. |
| lowerRightRow | number | Lower right row index |
| lowerRightColumn | number | Lower right column index |
### calculate() {#calculate--}
Calculates the custom position of plot area, axes if the position of them are auto assigned.
```javascript
calculate() : void;
```
### calculate(ChartCalculateOptions) {#calculate-chartcalculateoptions-}
Calculates the custom position of plot area, axes if the position of them are auto assigned, with Chart Calculate Options.
```javascript
calculate(calculateOptions: ChartCalculateOptions) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| calculateOptions | [ChartCalculateOptions](../chartcalculateoptions/) |  |
### toImageAsync(string) {#toImageAsync-string-}
Creates the chart image and saves it to a file. The extension of the file name determines the format of the image.
```javascript
toImageAsync(imageFile: string) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | string | The image file name with full path. |
**Returns**
[Promise<void>](../promise<void>/)
**Remarks**
The format of the image is specified by using the extension of the file name. For example, if you specify "myfile.png", then the image will be saved in the PNG format. The following file extensions are recognized: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.</p> If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.
### toImageAsync(string, ImageType) {#toImageAsync-string-imagetype-}
Creates the chart image and saves it to a file in the specified image type.
```javascript
toImageAsync(imageFile: string, imageType: ImageType) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | string | The image file name with full path. |
| imageType | [ImageType](../imagetype/) | The image type in which to save the image. |
**Returns**
[Promise<void>](../promise<void>/)
**Remarks**
The type of the image is specified by using <c>imageType</c>. The following types are supported: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.</p> If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.
### toImageAsync(string, number) {#toImageAsync-string-number-}
Creates the chart image and saves it to a file in the Jpeg format.
```javascript
toImageAsync(imageFile: string, jpegQuality: number) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | string | The image file name with full path. |
| jpegQuality | number | Jpeg quality. |
**Returns**
[Promise<void>](../promise<void>/)
**Remarks**
If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. NOTE: This method is now obsolete. Instead, please use ToImage(string,ImageOrPrintOptions) method with specified quality. This method will be removed 12 months later since March 2025. Aspose apologizes for any inconvenience you may have experienced.
### toImageAsync(number) {#toImageAsync-number-}
Creates the chart image and saves it to a stream in the Jpeg format.
```javascript
toImageAsync(jpegQuality: number) : Promise<Uint8Array>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| jpegQuality | number | Jpeg quality. |
**Returns**
The result stream
**Remarks**
If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.
### toImageAsync(ImageType) {#toImageAsync-imagetype-}
Creates the chart image and saves it to a stream in the specified format.
```javascript
toImageAsync(imageType: ImageType) : Promise<Uint8Array>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageType | [ImageType](../imagetype/) | The image type in which to save the image. |
**Returns**
The result stream
**Remarks**
The type of the image is specified by using <c>imageType</c>. The following types are supported: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.</p> If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.
### toImageAsync(string, ImageOrPrintOptions) {#toImageAsync-string-imageorprintoptions-}
Creates the chart image and saves it to a file. The extension of the file name determines the format of the image.
```javascript
toImageAsync(imageFile: string, options: ImageOrPrintOptions) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | string | The image file name with full path. |
| options | [ImageOrPrintOptions](../imageorprintoptions/) | Additional image creation options |
**Returns**
[Promise<void>](../promise<void>/)
**Remarks**
The format of the image is specified by using the extension of the file name. For example, if you specify "myfile.png", then the image will be saved in the PNG format. The following file extensions are recognized: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.</p> If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. Please refer to <a href="http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html">Supported Charts List</a> for more details.
### toImageAsync(ImageOrPrintOptions) {#toImageAsync-imageorprintoptions-}
Creates the chart image and saves it to a stream in the specified format.
```javascript
toImageAsync(options: ImageOrPrintOptions) : Promise<Uint8Array>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../imageorprintoptions/) | Additional image creation options |
**Returns**
The result stream
**Remarks**
The type of the image is specified by using <c>options.ImageType</c>. The following formats are supported: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.</p> If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. Please refer to <a href="http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html">Supported Charts List</a> for more details.
### toImage(string) {#toImage-string-}
Creates the chart image and saves it to a file. The extension of the file name determines the format of the image.
```javascript
toImage(imageFile: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | string | The image file name with full path. |
**Remarks**
The format of the image is specified by using the extension of the file name. For example, if you specify "myfile.png", then the image will be saved in the PNG format. The following file extensions are recognized: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.</p> If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.
### toImage(string, ImageType) {#toImage-string-imagetype-}
Creates the chart image and saves it to a file in the specified image type.
```javascript
toImage(imageFile: string, imageType: ImageType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | string | The image file name with full path. |
| imageType | [ImageType](../imagetype/) | The image type in which to save the image. |
**Remarks**
The type of the image is specified by using <c>imageType</c>. The following types are supported: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.</p> If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.
### toImage(string, number) {#toImage-string-number-}
Creates the chart image and saves it to a file in the Jpeg format.
```javascript
toImage(imageFile: string, jpegQuality: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | string | The image file name with full path. |
| jpegQuality | number | Jpeg quality. |
**Remarks**
If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. NOTE: This method is now obsolete. Instead, please use ToImage(string,ImageOrPrintOptions) method with specified quality. This method will be removed 12 months later since March 2025. Aspose apologizes for any inconvenience you may have experienced.
### toImage(number) {#toImage-number-}
Creates the chart image and saves it to a stream in the Jpeg format.
```javascript
toImage(jpegQuality: number) : Uint8Array;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| jpegQuality | number | Jpeg quality. |
**Returns**
The result stream
**Remarks**
If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.
### toImage(ImageType) {#toImage-imagetype-}
Creates the chart image and saves it to a stream in the specified format.
```javascript
toImage(imageType: ImageType) : Uint8Array;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageType | [ImageType](../imagetype/) | The image type in which to save the image. |
**Returns**
The result stream
**Remarks**
The type of the image is specified by using <c>imageType</c>. The following types are supported: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.</p> If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.
### toImage(string, ImageOrPrintOptions) {#toImage-string-imageorprintoptions-}
Creates the chart image and saves it to a file. The extension of the file name determines the format of the image.
```javascript
toImage(imageFile: string, options: ImageOrPrintOptions) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | string | The image file name with full path. |
| options | [ImageOrPrintOptions](../imageorprintoptions/) | Additional image creation options |
**Remarks**
The format of the image is specified by using the extension of the file name. For example, if you specify "myfile.png", then the image will be saved in the PNG format. The following file extensions are recognized: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.</p> If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. Please refer to <a href="http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html">Supported Charts List</a> for more details.
**Example**
Saves a chart to a png file with 400 x dpi and 300 y dpi.
```javascript
const { Workbook, ImageOrPrintOptions } = AsposeCells;
var options = new ImageOrPrintOptions();
options.horizontalResolution = 400;
options.verticalResolution = 300;
options.quality = 80;
var book = new Workbook(data);
var uint8Array = book.worksheets.get(0).charts.get(0).toImage(options);
```
### toImage(ImageOrPrintOptions) {#toImage-imageorprintoptions-}
Creates the chart image and saves it to a stream in the specified format.
```javascript
toImage(options: ImageOrPrintOptions) : Uint8Array;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../imageorprintoptions/) | Additional image creation options |
**Returns**
The result stream
**Remarks**
The type of the image is specified by using <c>options.ImageType</c>. The following formats are supported: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.</p> If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. Please refer to <a href="http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html">Supported Charts List</a> for more details.
**Example**
Saves a chart to an Uint8Array in jpeg file format with 400 x dpi and 300 y dpi.
```javascript
const fs = require("fs");
const { Workbook, ImageOrPrintOptions, ImageType } = AsposeCells;
var options = new ImageOrPrintOptions();
options.setImageType(ImageType.Jpeg);
options.horizontalResolution = 400;
options.verticalResolution = 300;
var book = new Workbook(data);
var uint8Array = book.worksheets.get(0).charts.get(0).toImage(options);
```
### toPdfAsync(string) {#toPdfAsync-string-}
Saves the chart to a pdf file.
```javascript
toPdfAsync(fileName: string) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | string | the pdf file name with full path |
**Returns**
[Promise<void>](../promise<void>/)
### toPdfAsync(string, number, number, PageLayoutAlignmentType, PageLayoutAlignmentType) {#toPdfAsync-string-number-number-pagelayoutalignmenttype-pagelayoutalignmenttype-}
Saves the chart to a pdf file.
```javascript
toPdfAsync(fileName: string, desiredPageWidth: number, desiredPageHeight: number, hAlignmentType: PageLayoutAlignmentType, vAlignmentType: PageLayoutAlignmentType) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | string | the pdf file name with full path |
| desiredPageWidth | number | The desired page width in inches. |
| desiredPageHeight | number | The desired page height in inches. |
| hAlignmentType | [PageLayoutAlignmentType](../pagelayoutalignmenttype/) | The chart horizontal alignment type in the output page. |
| vAlignmentType | [PageLayoutAlignmentType](../pagelayoutalignmenttype/) | The chart vertical alignment type in the output page. |
**Returns**
[Promise<void>](../promise<void>/)
### toPdfAsync() {#toPdfAsync--}
Creates the chart pdf and saves it to a stream.
```javascript
toPdfAsync() : Promise<Uint8Array>;
```
**Returns**
The result stream
### toPdfAsync(number, number, PageLayoutAlignmentType, PageLayoutAlignmentType) {#toPdfAsync-number-number-pagelayoutalignmenttype-pagelayoutalignmenttype-}
Creates the chart pdf and saves it to a stream.
```javascript
toPdfAsync(desiredPageWidth: number, desiredPageHeight: number, hAlignmentType: PageLayoutAlignmentType, vAlignmentType: PageLayoutAlignmentType) : Promise<Uint8Array>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| desiredPageWidth | number | The desired page width in inches. |
| desiredPageHeight | number | The desired page height in inches. |
| hAlignmentType | [PageLayoutAlignmentType](../pagelayoutalignmenttype/) | The chart horizontal alignment type in the output page. |
| vAlignmentType | [PageLayoutAlignmentType](../pagelayoutalignmenttype/) | The chart vertical alignment type in the output page. |
**Returns**
The result stream
### toPdf(string) {#toPdf-string-}
Saves the chart to a pdf file.
```javascript
toPdf(fileName: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | string | the pdf file name with full path |
### toPdf(string, number, number, PageLayoutAlignmentType, PageLayoutAlignmentType) {#toPdf-string-number-number-pagelayoutalignmenttype-pagelayoutalignmenttype-}
Saves the chart to a pdf file.
```javascript
toPdf(fileName: string, desiredPageWidth: number, desiredPageHeight: number, hAlignmentType: PageLayoutAlignmentType, vAlignmentType: PageLayoutAlignmentType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | string | the pdf file name with full path |
| desiredPageWidth | number | The desired page width in inches. |
| desiredPageHeight | number | The desired page height in inches. |
| hAlignmentType | [PageLayoutAlignmentType](../pagelayoutalignmenttype/) | The chart horizontal alignment type in the output page. |
| vAlignmentType | [PageLayoutAlignmentType](../pagelayoutalignmenttype/) | The chart vertical alignment type in the output page. |
### toPdf() {#toPdf--}
Creates the chart pdf and saves it to a stream.
```javascript
toPdf() : Uint8Array;
```
**Returns**
The result stream
### toPdf(number, number, PageLayoutAlignmentType, PageLayoutAlignmentType) {#toPdf-number-number-pagelayoutalignmenttype-pagelayoutalignmenttype-}
Creates the chart pdf and saves it to a stream.
```javascript
toPdf(desiredPageWidth: number, desiredPageHeight: number, hAlignmentType: PageLayoutAlignmentType, vAlignmentType: PageLayoutAlignmentType) : Uint8Array;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| desiredPageWidth | number | The desired page width in inches. |
| desiredPageHeight | number | The desired page height in inches. |
| hAlignmentType | [PageLayoutAlignmentType](../pagelayoutalignmenttype/) | The chart horizontal alignment type in the output page. |
| vAlignmentType | [PageLayoutAlignmentType](../pagelayoutalignmenttype/) | The chart vertical alignment type in the output page. |
**Returns**
The result stream
### getActualSize() {#getActualSize--}
Gets actual size of chart in unit of pixels.
```javascript
getActualSize() : number[];
```
**Returns**
Actual size in an array(width and height). [0] is width; [1] is height.
### hasAxis(AxisType, boolean) {#hasAxis-axistype-boolean-}
Returns which axes exist on the chart.
```javascript
hasAxis(aixsType: AxisType, isPrimary: boolean) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| aixsType | [AxisType](../axistype/) |  |
| isPrimary | boolean |  |
**Remarks**
Normally, Pie, PieExploded, PiePie,PieBar, Pie3D, Pie3DExploded,Doughnut, DoughnutExploded is no axis.
### switchRowColumn() {#switchRowColumn--}
Switches row/column.
```javascript
switchRowColumn() : boolean;
```
**Returns**
False means switching row/column fails.
### getChartDataRange() {#getChartDataRange--}
Gets the data source range of the chart.
```javascript
getChartDataRange() : string;
```
**Returns**
The data source.
**Remarks**
Only supports range.
### setChartDataRange(string, boolean) {#setChartDataRange-string-boolean-}
Specifies data range for a chart.
```javascript
setChartDataRange(area: string, isVertical: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | string | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
