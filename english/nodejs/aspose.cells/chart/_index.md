---
title: "Chart"
linktitle: "Chart"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Encapsulates the object that represents a single Excel chart."
type: docs
weight: 480
url: /nodejs/aspose.cells/chart/
---

## Chart class

Encapsulates the object that represents a single Excel chart.

## Methods

| Name | Description |
| --- | --- |
| [calculate()](#calculate) | Calculates the custom position of plot area, axes if the position of them are auto assigned. |
| [calculate()](#calculate-1) | Calculates the custom position of plot area, axes if the position of them are auto assigned, with Chart Calculate Option |
| [changeTemplate(data)](#changetemplate) | Change chart type with preset template. |
| [getActualChartSize()](#getactualchartsize) | Gets actual size of chart in unit of pixels. NOTE: This member is now obsolete. Instead, please use Chart.getActualSize( |
| [getActualSize()](#getactualsize) | Gets actual size of chart in unit of pixels. |
| [getAutoScaling()](#getautoscaling) | True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. The RightAngleAxes p |
| [getBackWall()](#getbackwall) | Returns a Walls object that represents the back wall of a 3-D chart. |
| [getCategoryAxis()](#getcategoryaxis) | Gets the chart's X axis. |
| [getChartArea()](#getchartarea) | Gets the chart area in the worksheet. |
| [getChartDataRange()](#getchartdatarange) | Gets the data source range of the chart. Only supports range. |
| [getChartDataTable()](#getchartdatatable) | Represents the chart data table. |
| [getChartObject()](#getchartobject) | Represents the chartShape; |
| [getChartShape()](#getchartshape) | Represents the chartShape; NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Charts.Chart.ChartObject  |
| [getDepthPercent()](#getdepthpercent) | Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent). |
| [getDisplayNaAsBlank()](#getdisplaynaasblank) | Indicates whether displaying #N/A as blank value. |
| [getElevation()](#getelevation) | Represents the elevation of the 3-D chart view, in degrees. The chart elevation is the height at which you view the char |
| [getFilteredNSeries()](#getfilterednseries) | Gets a SeriesCollection collection representing the data series that are filtered in the chart. |
| [getFirstSliceAngle()](#getfirstsliceangle) | Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies onl |
| [getFloor()](#getfloor) | Returns a Floor object that represents the walls of a 3-D chart. This property doesn't apply to 3-D pie charts. |
| [getGapDepth()](#getgapdepth) | Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width. The value of this |
| [getGapWidth()](#getgapwidth) | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this  |
| [getHeightPercent()](#getheightpercent) | Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent). |
| [getHidePivotFieldButtons()](#gethidepivotfieldbuttons) | Indicates whether hide the pivot chart field buttons only when the chart is PivotChart. |
| [getIs3D()](#getis3d) | Indicates whether the chart is a 3d chart. |
| [getLegend()](#getlegend) | Gets the chart legend. |
| [getLine()](#getline) | Gets the line. |
| [getNSeries()](#getnseries) | Gets a SeriesCollection collection representing the data series in the chart. |
| [getName()](#getname) | Gets and sets the name of the chart. |
| [getPageSetup()](#getpagesetup) | Represents the page setup description in this chart. |
| [getPerspective()](#getperspective) | Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100. This property is ignored if the Right |
| [getPivotOptions()](#getpivotoptions) | Specifies the pivot controls that appear on the chart |
| [getPivotSource()](#getpivotsource) | The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart. If the pivot table "Pivo |
| [getPlacement()](#getplacement) | Represents the way the chart is attached to the cells below it. The value of the property is PlacementType integer const |
| [getPlotArea()](#getplotarea) | Gets the chart's plot area which includes axis tick labels. |
| [getPlotBy()](#getplotby) | Gets and sets whether plot by row or column. The value of the property is PlotDataByType integer constant. |
| [getPlotEmptyCellsType()](#getplotemptycellstype) | Gets and sets how to plot the empty cells. The value of the property is PlotEmptyCellsType integer constant. |
| [getPlotVisibleCells()](#getplotvisiblecells) | Indicates whether only plot visible cells. NOTE: This member is now obsolete. Instead, please use PlotVisibleCellsOnly p |
| [getPlotVisibleCellsOnly()](#getplotvisiblecellsonly) | Indicates whether plot visible cells only. |
| [getPrintSize()](#getprintsize) | Gets and sets the printed chart size. The value of the property is PrintSizeType integer constant. |
| [getRightAngleAxes()](#getrightangleaxes) | True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie Charts). If this pro |
| [getRotationAngle()](#getrotationangle) | Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees). The value o |
| [getSecondCategoryAxis()](#getsecondcategoryaxis) | Gets the chart's second X axis. |
| [getSecondValueAxis()](#getsecondvalueaxis) | Gets the chart's second Y axis. |
| [getSeriesAxis()](#getseriesaxis) | Gets the chart's series axis. |
| [getShapes()](#getshapes) | Returns all drawing shapes in this chart. |
| [getShowDataTable()](#getshowdatatable) | Gets or sets a value indicating whether the chart displays a data table. |
| [getShowLegend()](#getshowlegend) | Gets or sets a value indicating whether the chart legend will be displayed. Default is true. |
| [getSideWall()](#getsidewall) | Returns a Walls object that represents the side wall of a 3-D chart. |
| [getSizeWithWindow()](#getsizewithwindow) | True if Microsoft Excel resizes the chart to match the size of the chart sheet window. |
| [getStyle()](#getstyle) | Gets and sets the builtin style. It should be between 1 and 48. Return -1 if it's not be set. |
| [getSubTitle()](#getsubtitle) | Gets the chart's sub-title. Only for ODS format file. |
| [getTitle()](#gettitle) | Gets the chart's title. |
| [getType()](#gettype) | Gets or sets a chart's type. The value of the property is ChartType integer constant. |
| [getValueAxis()](#getvalueaxis) | Gets the chart's Y axis. |
| [getWalls()](#getwalls) | Returns a Walls object that represents the walls of a 3-D chart. This property doesn't apply to 3-D pie charts. |
| [getWallsAndGridlines2D()](#getwallsandgridlines2d) | True if gridlines are drawn two-dimensionally on a 3-D chart. |
| [getWorksheet()](#getworksheet) | Gets the worksheet which contains this chart. |
| [hasAxis()](#hasaxis) | Returns which axes exist on the chart. Normally, Pie, PieExploded, PiePie,PieBar, Pie3D, Pie3DExploded,Doughnut, Doughnu |
| [isCellReferedByChart(sheetIndex, rowIndex, columnIndex)](#iscellreferedbychart) | Returns whether the cell refered by the chart. |
| [isChartDataChanged()](#ischartdatachanged) | Detects if a chart's data source has changed. The method detects the changes in the chart's data source before rendering |
| [isRectangularCornered()](#isrectangularcornered) | Gets or sets a value indicating whether the chart area is rectangular cornered. Default is true. |
| [isReferedByChart(rowIndex, columnIndex)](#isreferedbychart) | Returns whether the cell refered by the chart. NOTE: This method is now obsolete. Instead, please use IsCellReferedByCha |
| [move(upperLeftColumn, upperLeftRow, lowerRightColumn, lowerRightRow)](#move) | Moves the chart to a specified location. |
| [refreshPivotData()](#refreshpivotdata) | Refreshes chart's data from pivot table. We will gather data from pivot data source to the pivot table report. This meth |
| [setAutoScaling()](#setautoscaling) | True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. The RightAngleAxes p |
| [setChartDataRange(area, isVertical)](#setchartdatarange) | Specifies data range for a chart. |
| [setDepthPercent()](#setdepthpercent) | Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent). |
| [setDisplayNaAsBlank()](#setdisplaynaasblank) | Indicates whether displaying #N/A as blank value. |
| [setElevation()](#setelevation) | Represents the elevation of the 3-D chart view, in degrees. The chart elevation is the height at which you view the char |
| [setFirstSliceAngle()](#setfirstsliceangle) | Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies onl |
| [setGapDepth()](#setgapdepth) | Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width. The value of this |
| [setGapWidth()](#setgapwidth) | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this  |
| [setHeightPercent()](#setheightpercent) | Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent). |
| [setHidePivotFieldButtons()](#sethidepivotfieldbuttons) | Indicates whether hide the pivot chart field buttons only when the chart is PivotChart. |
| [setName()](#setname) | Gets and sets the name of the chart. |
| [setPerspective()](#setperspective) | Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100. This property is ignored if the Right |
| [setPivotSource()](#setpivotsource) | The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart. If the pivot table "Pivo |
| [setPlacement()](#setplacement) | Represents the way the chart is attached to the cells below it. The value of the property is PlacementType integer const |
| [setPlotEmptyCellsType()](#setplotemptycellstype) | Gets and sets how to plot the empty cells. The value of the property is PlotEmptyCellsType integer constant. |
| [setPlotVisibleCells()](#setplotvisiblecells) | Indicates whether only plot visible cells. NOTE: This member is now obsolete. Instead, please use PlotVisibleCellsOnly p |
| [setPlotVisibleCellsOnly()](#setplotvisiblecellsonly) | Indicates whether plot visible cells only. |
| [setPrintSize()](#setprintsize) | Gets and sets the printed chart size. The value of the property is PrintSizeType integer constant. |
| [setRectangularCornered()](#setrectangularcornered) | Gets or sets a value indicating whether the chart area is rectangular cornered. Default is true. |
| [setRightAngleAxes()](#setrightangleaxes) | True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie Charts). If this pro |
| [setRotationAngle()](#setrotationangle) | Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees). The value o |
| [setShowDataTable()](#setshowdatatable) | Gets or sets a value indicating whether the chart displays a data table. |
| [setShowLegend()](#setshowlegend) | Gets or sets a value indicating whether the chart legend will be displayed. Default is true. |
| [setSizeWithWindow()](#setsizewithwindow) | True if Microsoft Excel resizes the chart to match the size of the chart sheet window. |
| [setStyle()](#setstyle) | Gets and sets the builtin style. It should be between 1 and 48. Return -1 if it's not be set. |
| [setType()](#settype) | Gets or sets a chart's type. The value of the property is ChartType integer constant. |
| [setWallsAndGridlines2D()](#setwallsandgridlines2d) | True if gridlines are drawn two-dimensionally on a 3-D chart. |
| [switchRowColumn()](#switchrowcolumn) | Switches row/column. |
| [toImage(imageFile)](#toimage) | Creates the chart image and saves it to a file. The extension of the file name determines the format of the image. The f |
| [toImage(imageFile, imageFormat)](#toimage-1) | Creates the chart image and saves it to a file in the specified format. NOTE: This member is now obsolete. Instead, plea |
| [toImage(imageFile, imageType)](#toimage-2) | Creates the chart image and saves it to a file in the specified image type. The type of the image is specified by using  |
| [toImage(imageFile, jpegQuality)](#toimage-3) | Creates the chart image and saves it to a file in the Jpeg format. If the width or height is zero or the chart is not su |
| [toImage(imageFile, options)](#toimage-4) | Creates the chart image and saves it to a file. The extension of the file name determines the format of the image. The f |
| [toPdf(fileName)](#topdf) | Saves the chart to a pdf file. |
| [toPdf(fileName, desiredPageWidth, desiredPageHeight, hAlignmentType, vAlignmentType)](#topdf-1) | Saves the chart to a pdf file. |
| [toImageStream(chart, stream, options)](#toimagestream) *(static)* | Creates the chart image and saves it to a stream in the specified format. The format of the image is specified by using  |
| [toPdfStream(chart, stream)](#topdfstream) *(static)* | Creates the chart pdf and saves it to a stream. |

### calculate() {#calculate}

Calculates the custom position of plot area, axes if the position of them are auto assigned.

### calculate() {#calculate-1}

Calculates the custom position of plot area, axes if the position of them are auto assigned, with Chart Calculate Options.

### changeTemplate(data) {#changetemplate}

Change chart type with preset template.

| Parameter | Type | Description |
| --- | --- | --- |
| data | Array of byte | The data of chart template file(.crtx). |

### getActualChartSize() {#getactualchartsize}

Gets actual size of chart in unit of pixels. NOTE: This member is now obsolete. Instead, please use Chart.getActualSize() method. This property will be removed 12 months later since July 2022. Aspose apologizes for any inconvenience you may have experienced.@return {Number[]} Actual size in an array(width and height). [0] is width; [1] is height.

### getActualSize() {#getactualsize}

Gets actual size of chart in unit of pixels.

**Returns:** Array of Number — `Array of Number` Actual size in an array(width and height). [0] is width; [1] is height.

### getAutoScaling() {#getautoscaling}

True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. The RightAngleAxes property must be True.

### getBackWall() {#getbackwall}

Returns a Walls object that represents the back wall of a 3-D chart.

### getCategoryAxis() {#getcategoryaxis}

Gets the chart's X axis.

### getChartArea() {#getchartarea}

Gets the chart area in the worksheet.

### getChartDataRange() {#getchartdatarange}

Gets the data source range of the chart. Only supports range.

**Returns:** String — `String` The data source.

### getChartDataTable() {#getchartdatatable}

Represents the chart data table.

### getChartObject() {#getchartobject}

Represents the chartShape;

### getChartShape() {#getchartshape}

Represents the chartShape; NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Charts.Chart.ChartObject property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

### getDepthPercent() {#getdepthpercent}

Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent).

### getDisplayNaAsBlank() {#getdisplaynaasblank}

Indicates whether displaying #N/A as blank value.

### getElevation() {#getelevation}

Represents the elevation of the 3-D chart view, in degrees. The chart elevation is the height at which you view the chart, in degrees. The default is 15 for most chart types. The value of this property must be between -90 and 90, except for 3-D bar charts, where it must be between 0 and 44.

### getFilteredNSeries() {#getfilterednseries}

Gets a SeriesCollection collection representing the data series that are filtered in the chart.

### getFirstSliceAngle() {#getfirstsliceangle}

Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.

### getFloor() {#getfloor}

Returns a Floor object that represents the walls of a 3-D chart. This property doesn't apply to 3-D pie charts.

### getGapDepth() {#getgapdepth}

Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width. The value of this property must be between 0 and 500.

### getGapWidth() {#getgapwidth}

Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500.

### getHeightPercent() {#getheightpercent}

Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent).

### getHidePivotFieldButtons() {#gethidepivotfieldbuttons}

Indicates whether hide the pivot chart field buttons only when the chart is PivotChart.

### getIs3D() {#getis3d}

Indicates whether the chart is a 3d chart.

### getLegend() {#getlegend}

Gets the chart legend.

### getLine() {#getline}

Gets the line.

### getNSeries() {#getnseries}

Gets a SeriesCollection collection representing the data series in the chart.

### getName() {#getname}

Gets and sets the name of the chart.

### getPageSetup() {#getpagesetup}

Represents the page setup description in this chart.

### getPerspective() {#getperspective}

Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100. This property is ignored if the RightAngleAxes property is True.

### getPivotOptions() {#getpivotoptions}

Specifies the pivot controls that appear on the chart

### getPivotSource() {#getpivotsource}

The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart. If the pivot table "PivotTable1" in the Worksheet "Sheet1" in the file "Book1.xls". The pivotSource could be "[Book1.xls]Sheet1!PivotTable1" if the chart and the PivotTable is not in the same workbook. If you set this property ,the previous data source setting will be lost.

### getPlacement() {#getplacement}

Represents the way the chart is attached to the cells below it. The value of the property is PlacementType integer constant.

### getPlotArea() {#getplotarea}

Gets the chart's plot area which includes axis tick labels.

### getPlotBy() {#getplotby}

Gets and sets whether plot by row or column. The value of the property is PlotDataByType integer constant.

### getPlotEmptyCellsType() {#getplotemptycellstype}

Gets and sets how to plot the empty cells. The value of the property is PlotEmptyCellsType integer constant.

### getPlotVisibleCells() {#getplotvisiblecells}

Indicates whether only plot visible cells. NOTE: This member is now obsolete. Instead, please use PlotVisibleCellsOnly property. This method will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

### getPlotVisibleCellsOnly() {#getplotvisiblecellsonly}

Indicates whether plot visible cells only.

### getPrintSize() {#getprintsize}

Gets and sets the printed chart size. The value of the property is PrintSizeType integer constant.

### getRightAngleAxes() {#getrightangleaxes}

True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie Charts). If this property is True, the Perspective property is ignored.

### getRotationAngle() {#getrotationangle}

Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees). The value of this property must be from 0 to 360, except for 3-D bar charts, where the value must be from 0 to 44. The default value is 20. Applies only to 3-D charts.

### getSecondCategoryAxis() {#getsecondcategoryaxis}

Gets the chart's second X axis.

### getSecondValueAxis() {#getsecondvalueaxis}

Gets the chart's second Y axis.

### getSeriesAxis() {#getseriesaxis}

Gets the chart's series axis.

### getShapes() {#getshapes}

Returns all drawing shapes in this chart.

### getShowDataTable() {#getshowdatatable}

Gets or sets a value indicating whether the chart displays a data table.

### getShowLegend() {#getshowlegend}

Gets or sets a value indicating whether the chart legend will be displayed. Default is true.

### getSideWall() {#getsidewall}

Returns a Walls object that represents the side wall of a 3-D chart.

### getSizeWithWindow() {#getsizewithwindow}

True if Microsoft Excel resizes the chart to match the size of the chart sheet window.

### getStyle() {#getstyle}

Gets and sets the builtin style. It should be between 1 and 48. Return -1 if it's not be set.

### getSubTitle() {#getsubtitle}

Gets the chart's sub-title. Only for ODS format file.

### getTitle() {#gettitle}

Gets the chart's title.

### getType() {#gettype}

Gets or sets a chart's type. The value of the property is ChartType integer constant.

### getValueAxis() {#getvalueaxis}

Gets the chart's Y axis.

### getWalls() {#getwalls}

Returns a Walls object that represents the walls of a 3-D chart. This property doesn't apply to 3-D pie charts.

### getWallsAndGridlines2D() {#getwallsandgridlines2d}

True if gridlines are drawn two-dimensionally on a 3-D chart.

### getWorksheet() {#getworksheet}

Gets the worksheet which contains this chart.

### hasAxis() {#hasaxis}

Returns which axes exist on the chart. Normally, Pie, PieExploded, PiePie,PieBar, Pie3D, Pie3DExploded,Doughnut, DoughnutExploded is no axis.

### isCellReferedByChart(sheetIndex, rowIndex, columnIndex) {#iscellreferedbychart}

Returns whether the cell refered by the chart.

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Number | The sheet Index.-1 means the worksheet which contains current chart. |
| rowIndex | Number | The row index |
| columnIndex | Number | The column index |

**Returns:** boolean — `boolean`

### isChartDataChanged() {#ischartdatachanged}

Detects if a chart's data source has changed. The method detects the changes in the chart's data source before rendering the chart to image format. At first Chart.toImage call, the chart source data (e.g. XValuesParseData, ValuesParseData) will be recorded. Before calling the Chart.toImage method again, call IsChartDataChanged method to check if Chart needs re-rendering.

**Returns:** boolean — `boolean` Returns true if the chart has changed otherwise returns false

### isRectangularCornered() {#isrectangularcornered}

Gets or sets a value indicating whether the chart area is rectangular cornered. Default is true.

### isReferedByChart(rowIndex, columnIndex) {#isreferedbychart}

Returns whether the cell refered by the chart. NOTE: This method is now obsolete. Instead, please use IsCellReferedByChart(int,int,int) method. This method will be removed 12 months later since April 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Number | The row index |
| columnIndex | Number | The column index |

**Returns:** boolean — `boolean`

### move(upperLeftColumn, upperLeftRow, lowerRightColumn, lowerRightRow) {#move}

Moves the chart to a specified location.

| Parameter | Description |
| --- | --- |
| upperLeftColumn | Upper left column index. |
| upperLeftRow | Upper left row index. |
| lowerRightColumn | Lower right column index |
| lowerRightRow | Lower right row index |

### refreshPivotData() {#refreshpivotdata}

Refreshes chart's data from pivot table. We will gather data from pivot data source to the pivot table report. This method is only used to gather all data to a pivot chart.

### setAutoScaling() {#setautoscaling}

True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. The RightAngleAxes property must be True.

### setChartDataRange(area, isVertical) {#setchartdatarange}

Specifies data range for a chart.

| Parameter | Type | Description |
| --- | --- | --- |
| area | String | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |

### setDepthPercent() {#setdepthpercent}

Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent).

### setDisplayNaAsBlank() {#setdisplaynaasblank}

Indicates whether displaying #N/A as blank value.

### setElevation() {#setelevation}

Represents the elevation of the 3-D chart view, in degrees. The chart elevation is the height at which you view the chart, in degrees. The default is 15 for most chart types. The value of this property must be between -90 and 90, except for 3-D bar charts, where it must be between 0 and 44.

### setFirstSliceAngle() {#setfirstsliceangle}

Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.

### setGapDepth() {#setgapdepth}

Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width. The value of this property must be between 0 and 500.

### setGapWidth() {#setgapwidth}

Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500.

### setHeightPercent() {#setheightpercent}

Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent).

### setHidePivotFieldButtons() {#sethidepivotfieldbuttons}

Indicates whether hide the pivot chart field buttons only when the chart is PivotChart.

### setName() {#setname}

Gets and sets the name of the chart.

### setPerspective() {#setperspective}

Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100. This property is ignored if the RightAngleAxes property is True.

### setPivotSource() {#setpivotsource}

The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart. If the pivot table "PivotTable1" in the Worksheet "Sheet1" in the file "Book1.xls". The pivotSource could be "[Book1.xls]Sheet1!PivotTable1" if the chart and the PivotTable is not in the same workbook. If you set this property ,the previous data source setting will be lost.

### setPlacement() {#setplacement}

Represents the way the chart is attached to the cells below it. The value of the property is PlacementType integer constant.

### setPlotEmptyCellsType() {#setplotemptycellstype}

Gets and sets how to plot the empty cells. The value of the property is PlotEmptyCellsType integer constant.

### setPlotVisibleCells() {#setplotvisiblecells}

Indicates whether only plot visible cells. NOTE: This member is now obsolete. Instead, please use PlotVisibleCellsOnly property. This method will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

### setPlotVisibleCellsOnly() {#setplotvisiblecellsonly}

Indicates whether plot visible cells only.

### setPrintSize() {#setprintsize}

Gets and sets the printed chart size. The value of the property is PrintSizeType integer constant.

### setRectangularCornered() {#setrectangularcornered}

Gets or sets a value indicating whether the chart area is rectangular cornered. Default is true.

### setRightAngleAxes() {#setrightangleaxes}

True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie Charts). If this property is True, the Perspective property is ignored.

### setRotationAngle() {#setrotationangle}

Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees). The value of this property must be from 0 to 360, except for 3-D bar charts, where the value must be from 0 to 44. The default value is 20. Applies only to 3-D charts.

### setShowDataTable() {#setshowdatatable}

Gets or sets a value indicating whether the chart displays a data table.

### setShowLegend() {#setshowlegend}

Gets or sets a value indicating whether the chart legend will be displayed. Default is true.

### setSizeWithWindow() {#setsizewithwindow}

True if Microsoft Excel resizes the chart to match the size of the chart sheet window.

### setStyle() {#setstyle}

Gets and sets the builtin style. It should be between 1 and 48. Return -1 if it's not be set.

### setType() {#settype}

Gets or sets a chart's type. The value of the property is ChartType integer constant.

### setWallsAndGridlines2D() {#setwallsandgridlines2d}

True if gridlines are drawn two-dimensionally on a 3-D chart.

### switchRowColumn() {#switchrowcolumn}

Switches row/column.

**Returns:** boolean — `boolean` False means switching row/column fails.

### toImage(imageFile) {#toimage}

Creates the chart image and saves it to a file. The extension of the file name determines the format of the image. The format of the image is specified by using the extension of the file name. For example, if you specify "myfile.png", then the image will be saved in the PNG format. The following file extensions are recognized: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf. If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.

| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | String | The image file name with full path. |

### toImage(imageFile, imageFormat) {#toimage-1}

Creates the chart image and saves it to a file in the specified format. NOTE: This member is now obsolete. Instead, please use Chart.ToImage(string, ImageType) method. This property will be removed 12 months later since July 2022. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | String | The image file name with full path. |
| imageFormat | ImageFormat | The format in which to save the image. |

### toImage(imageFile, imageType) {#toimage-2}

Creates the chart image and saves it to a file in the specified image type. The type of the image is specified by using imageType. The following types are supported: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf. If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.

| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | String | The image file name with full path. |
| imageType | Number | ImageType |

### toImage(imageFile, jpegQuality) {#toimage-3}

Creates the chart image and saves it to a file in the Jpeg format. If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.

| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | String | The image file name with full path. |
| jpegQuality | long | Jpeg quality. |

### toImage(imageFile, options) {#toimage-4}

Creates the chart image and saves it to a file. The extension of the file name determines the format of the image. The format of the image is specified by using the extension of the file name. For example, if you specify "myfile.png", then the image will be saved in the PNG format. The following file extensions are recognized: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf. If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. Please refer to Supported Charts List for more details.

| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | String | The image file name with full path. |
| options | ImageOrPrintOptions | Additional image creation options |

**Example:**

```js
var options = new aspose.cells.ImageOrPrintOptions();
options.setHorizontalResolution(300);
options.setVerticalResolution(300);
var book = new aspose.cells.Workbook("Book1.xls");
book.getWorksheets().get(0).getCharts().get(0).toImage("chart.png", options);
```

### toPdf(fileName) {#topdf}

Saves the chart to a pdf file.

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | the pdf file name with full path |

### toPdf(fileName, desiredPageWidth, desiredPageHeight, hAlignmentType, vAlignmentType) {#topdf-1}

Saves the chart to a pdf file.

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | the pdf file name with full path |
| desiredPageWidth | Number | The desired page width in inches. |
| desiredPageHeight | Number | The desired page height in inches. |
| hAlignmentType | Number | PageLayoutAlignmentType |
| vAlignmentType | Number | PageLayoutAlignmentType |

### toImageStream(chart, stream, options) (static) {#toimagestream}

Creates the chart image and saves it to a stream in the specified format. The format of the image is specified by using options.ImageFormat. The following formats are supported: ImageFormat.Bmp, ImageFormat.Gif, ImageFormat.Png, ImageFormat.Jpeg, ImageFormat.Tiff, ImageFormat.Emf. If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. Please refer to Supported Charts List for more details.

| Parameter | Type | Description |
| --- | --- | --- |
| chart | Chart | The Chart object |
| stream | WritableStream | The stream of the output image |
| options | ImageOrPrintOptions | Addtional image creation options |

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook("Book2.xlsx");
var imgOptions = new aspose.cells.ImageOrPrintOptions();
imgOptions.setHorizontalResolution(200);
imgOptions.setVerticalResolution(300);
imgOptions.setImageFormat(aspose.cells.ImageFormat.getJpeg());
imgWriteStream = fs.createWriteStream("chart.jpeg");
var chart = workbook.getWorksheets().get("Chart").getCharts().get(0);
aspose.cells.Chart.toImageStream(chart, imgWriteStream, imgOptions);
```

### toPdfStream(chart, stream) (static) {#topdfstream}

Creates the chart pdf and saves it to a stream.

| Parameter | Type | Description |
| --- | --- | --- |
| chart | Chart | The Chart object |
| stream | WritableStream | The output stream |

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook("Book2.xlsx");
var chart = workbook.getWorksheets().get("Chart").getCharts().get(0);
var imgWriteStream = fs.createWriteStream("chart.pdf");
aspose.cells.Chart.toPdfStream(chart, imgWriteStream);
```
