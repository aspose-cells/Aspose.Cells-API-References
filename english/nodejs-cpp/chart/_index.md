﻿---
title: Chart
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents a single Excel chart.
type: docs
url: /nodejs-cpp/chart/
---

## Chart class

Encapsulates the object that represents a single Excel chart.

```javascript
class Chart;
```


## Methods

| Method | Description |
| --- | --- |
| [getStyle()](#getStyle--)| Gets and sets the builtin style. |
| [setStyle(number)](#setStyle-number-)| Gets and sets the builtin style. |
| [getChartObject()](#getChartObject--)| Represents the chartShape; |
| [getHidePivotFieldButtons()](#getHidePivotFieldButtons--)| Indicates whether hide the pivot chart field buttons only when the chart is PivotChart. |
| [setHidePivotFieldButtons(boolean)](#setHidePivotFieldButtons-boolean-)| Indicates whether hide the pivot chart field buttons only when the chart is PivotChart. |
| [getPivotOptions()](#getPivotOptions--)| Specifies the pivot controls that appear on the chart |
| [getPivotSource()](#getPivotSource--)| The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart. |
| [setPivotSource(string)](#setPivotSource-string-)| The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart. |
| [getPlotBy()](#getPlotBy--)| Gets and sets whether plot by row or column. |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--)| Gets and sets  how to plot the empty cells. |
| [setPlotEmptyCellsType(PlotEmptyCellsType)](#setPlotEmptyCellsType-plotemptycellstype-)| Gets and sets  how to plot the empty cells. |
| [getPlotVisibleCellsOnly()](#getPlotVisibleCellsOnly--)| Indicates whether plot visible cells only. |
| [setPlotVisibleCellsOnly(boolean)](#setPlotVisibleCellsOnly-boolean-)| Indicates whether plot visible cells only. |
| [getDisplayNaAsBlank()](#getDisplayNaAsBlank--)| Indicates whether displaying #N/A as blank value. |
| [setDisplayNaAsBlank(boolean)](#setDisplayNaAsBlank-boolean-)| Indicates whether displaying #N/A as blank value. |
| [getName()](#getName--)| Gets and sets the name of the chart. |
| [setName(string)](#setName-string-)| Gets and sets the name of the chart. |
| [getSizeWithWindow()](#getSizeWithWindow--)| True if Microsoft Excel resizes the chart to match the size of the chart sheet window. |
| [setSizeWithWindow(boolean)](#setSizeWithWindow-boolean-)| True if Microsoft Excel resizes the chart to match the size of the chart sheet window. |
| [getWorksheet()](#getWorksheet--)| Gets the worksheet which contains this chart. |
| [getShapes()](#getShapes--)| Returns all drawing shapes in this chart. |
| [getPrintSize()](#getPrintSize--)| Gets and sets the printed chart size. |
| [setPrintSize(PrintSizeType)](#setPrintSize-printsizetype-)| Gets and sets the printed chart size. |
| [getType()](#getType--)| Gets or sets a chart's type. |
| [setType(ChartType)](#setType-charttype-)| Gets or sets a chart's type. |
| [getNSeries()](#getNSeries--)| Gets a [SeriesCollection](../seriescollection/) collection representing the data series in the chart. |
| [getFilteredNSeries()](#getFilteredNSeries--)| Gets a [SeriesCollection](../seriescollection/) collection representing the data series that are filtered in the chart. |
| [getTitle()](#getTitle--)| Gets the chart's title. |
| [getSubTitle()](#getSubTitle--)| Gets the chart's sub-title. Only for ODS format file. |
| [getPlotArea()](#getPlotArea--)| Gets the chart's plot area which includes axis tick labels. |
| [getChartArea()](#getChartArea--)| Gets the chart area in the worksheet. |
| [getCategoryAxis()](#getCategoryAxis--)| Gets the chart's X axis. |
| [getValueAxis()](#getValueAxis--)| Gets the chart's Y axis. |
| [getSecondValueAxis()](#getSecondValueAxis--)| Gets the chart's second Y axis. |
| [getSecondCategoryAxis()](#getSecondCategoryAxis--)| Gets the chart's second X axis. |
| [getSeriesAxis()](#getSeriesAxis--)| Gets the chart's series axis. |
| [getLegend()](#getLegend--)| Gets the chart legend. |
| [getChartDataTable()](#getChartDataTable--)| Represents the chart data table. |
| [getShowLegend()](#getShowLegend--)| Gets or sets a value indicating whether the chart legend will be displayed. Default is true. |
| [setShowLegend(boolean)](#setShowLegend-boolean-)| Gets or sets a value indicating whether the chart legend will be displayed. Default is true. |
| [isRectangularCornered()](#isRectangularCornered--)| Gets or sets a value indicating whether the chart area is rectangular cornered. Default is true. |
| [setIsRectangularCornered(boolean)](#setIsRectangularCornered-boolean-)| Gets or sets a value indicating whether the chart area is rectangular cornered. Default is true. |
| [getShowDataTable()](#getShowDataTable--)| Gets or sets a value indicating whether the chart displays a data table. |
| [setShowDataTable(boolean)](#setShowDataTable-boolean-)| Gets or sets a value indicating whether the chart displays a data table. |
| [getFirstSliceAngle()](#getFirstSliceAngle--)| Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360. |
| [setFirstSliceAngle(number)](#setFirstSliceAngle-number-)| Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360. |
| [getGapWidth()](#getGapWidth--)| Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500. |
| [setGapWidth(number)](#setGapWidth-number-)| Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500. |
| [getGapDepth()](#getGapDepth--)| Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width. The value of this property must be between 0 and 500. |
| [setGapDepth(number)](#setGapDepth-number-)| Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width. The value of this property must be between 0 and 500. |
| [getFloor()](#getFloor--)| Returns a [Floor](../floor/) object that represents the walls of a 3-D chart. |
| [getWalls()](#getWalls--)| Returns a [Walls](../walls/) object that represents the walls of a 3-D chart. |
| [getBackWall()](#getBackWall--)| Returns a [Walls](../walls/) object that represents the back wall of a 3-D chart. |
| [getSideWall()](#getSideWall--)| Returns a [Walls](../walls/) object that represents the side wall of a 3-D chart. |
| [getWallsAndGridlines2D()](#getWallsAndGridlines2D--)| True if gridlines are drawn two-dimensionally on a 3-D chart. |
| [setWallsAndGridlines2D(boolean)](#setWallsAndGridlines2D-boolean-)| True if gridlines are drawn two-dimensionally on a 3-D chart. |
| [getRotationAngle()](#getRotationAngle--)| Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees). |
| [setRotationAngle(number)](#setRotationAngle-number-)| Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees). |
| [getElevation()](#getElevation--)| Represents the elevation of the 3-D chart view, in degrees. |
| [setElevation(number)](#setElevation-number-)| Represents the elevation of the 3-D chart view, in degrees. |
| [getRightAngleAxes()](#getRightAngleAxes--)| True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie Charts). |
| [setRightAngleAxes(boolean)](#setRightAngleAxes-boolean-)| True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie Charts). |
| [getAutoScaling()](#getAutoScaling--)| True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. The RightAngleAxes property must be True. |
| [setAutoScaling(boolean)](#setAutoScaling-boolean-)| True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. The RightAngleAxes property must be True. |
| [getHeightPercent()](#getHeightPercent--)| Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent). |
| [setHeightPercent(number)](#setHeightPercent-number-)| Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent). |
| [getPerspective()](#getPerspective--)| Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100. This property is ignored if the RightAngleAxes property is True. |
| [setPerspective(number)](#setPerspective-number-)| Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100. This property is ignored if the RightAngleAxes property is True. |
| [getIs3D()](#getIs3D--)| Indicates whether the chart is a 3d chart. |
| [getDepthPercent()](#getDepthPercent--)| Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent). |
| [setDepthPercent(number)](#setDepthPercent-number-)| Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent). |
| [getPlacement()](#getPlacement--)| Represents the way the chart is attached to the cells below it. |
| [setPlacement(PlacementType)](#setPlacement-placementtype-)| Represents the way the chart is attached to the cells below it. |
| [getPageSetup()](#getPageSetup--)| Represents the page setup description in this chart. |
| [getLine()](#getLine--)| Gets the line. |
| [isCellReferedByChart(number, number, number)](#isCellReferedByChart-number-number-number-)| Returns whether the cell refered by the chart. |
| [isChartDataChanged()](#isChartDataChanged--)| Detects if a chart's data source has changed. |
| [refreshPivotData()](#refreshPivotData--)| Refreshes chart's data from pivot table. |
| [changeTemplate(number[])](#changeTemplate-numberarray-)| Change chart type with preset template. |
| [move(number, number, number, number)](#move-number-number-number-number-)| Moves the chart to a specified location. |
| [calculate()](#calculate--)| Calculates the custom position of plot area, axes if the position of them are auto assigned. |
| [calculate(ChartCalculateOptions)](#calculate-chartcalculateoptions-)| Calculates the custom position of plot area, axes if the position of them are auto assigned, with Chart Calculate Options. |
| [toImage(string)](#toImage-string-)| Creates the chart image and saves it to a file. The extension of the file name determines the format of the image. |
| [toImage(string, ImageType)](#toImage-string-imagetype-)| Creates the chart image and saves it to a file in the specified image type. |
| [toImage(string, number)](#toImage-string-number-)| Creates the chart image and saves it to a file in the Jpeg format. |
| [toImage(number)](#toImage-number-)| Creates the chart image and saves it to a stream in the Jpeg format. |
| [toImage(ImageType)](#toImage-imagetype-)| Creates the chart image and saves it to a stream in the specified format. |
| [toImage(string, ImageOrPrintOptions)](#toImage-string-imageorprintoptions-)| Creates the chart image and saves it to a file. The extension of the file name determines the format of the image. |
| [toImage(ImageOrPrintOptions)](#toImage-imageorprintoptions-)| Creates the chart image and saves it to a stream in the specified format. |
| [toPdf(string)](#toPdf-string-)| Saves the chart to a pdf file. |
| [toPdf(string, number, number, PageLayoutAlignmentType, PageLayoutAlignmentType)](#toPdf-string-number-number-pagelayoutalignmenttype-pagelayoutalignmenttype-)| Saves the chart to a pdf file. |
| [toPdf()](#toPdf--)| Creates the chart pdf and saves it to a stream. |
| [toPdf(number, number, PageLayoutAlignmentType, PageLayoutAlignmentType)](#toPdf-number-number-pagelayoutalignmenttype-pagelayoutalignmenttype-)| Creates the chart pdf and saves it to a stream. |
| [getActualSize()](#getActualSize--)| Gets actual size of chart in unit of pixels. |
| [hasAxis(AxisType, boolean)](#hasAxis-axistype-boolean-)| Returns which axes exist on the chart. |
| [switchRowColumn()](#switchRowColumn--)| Switches row/column. |
| [getChartDataRange()](#getChartDataRange--)| Gets the data source range of the chart. |
| [setChartDataRange(string, boolean)](#setChartDataRange-string-boolean-)| Specifies data range for a chart. |


### getStyle() {#getStyle--}

Gets and sets the builtin style.

```javascript
getStyle() : number;
```


**Remarks**

It should be between 1 and 48. Return -1 if it's not be set.

### setStyle(number) {#setStyle-number-}

Gets and sets the builtin style.

```javascript
setStyle(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

It should be between 1 and 48. Return -1 if it's not be set.

### getChartObject() {#getChartObject--}

Represents the chartShape;

```javascript
getChartObject() : ChartShape;
```


**Returns**

[ChartShape](../chartshape/)

### getHidePivotFieldButtons() {#getHidePivotFieldButtons--}

Indicates whether hide the pivot chart field buttons only when the chart is PivotChart.

```javascript
getHidePivotFieldButtons() : boolean;
```


### setHidePivotFieldButtons(boolean) {#setHidePivotFieldButtons-boolean-}

Indicates whether hide the pivot chart field buttons only when the chart is PivotChart.

```javascript
setHidePivotFieldButtons(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPivotOptions() {#getPivotOptions--}

Specifies the pivot controls that appear on the chart

```javascript
getPivotOptions() : PivotOptions;
```


**Returns**

[PivotOptions](../pivotoptions/)

### getPivotSource() {#getPivotSource--}

The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart.

```javascript
getPivotSource() : string;
```


**Remarks**

If the pivot table  "PivotTable1" in the Worksheet "Sheet1" in the file "Book1.xls". The pivotSource could be "[Book1.xls]Sheet1!PivotTable1" if the chart and the PivotTable is not in the same workbook. If you set this property ,the previous data source setting will be lost.

### setPivotSource(string) {#setPivotSource-string-}

The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart.

```javascript
setPivotSource(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

If the pivot table  "PivotTable1" in the Worksheet "Sheet1" in the file "Book1.xls". The pivotSource could be "[Book1.xls]Sheet1!PivotTable1" if the chart and the PivotTable is not in the same workbook. If you set this property ,the previous data source setting will be lost.

### getPlotBy() {#getPlotBy--}

Gets and sets whether plot by row or column.

```javascript
getPlotBy() : PlotDataByType;
```


**Returns**

[PlotDataByType](../plotdatabytype/)

### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}

Gets and sets  how to plot the empty cells.

```javascript
getPlotEmptyCellsType() : PlotEmptyCellsType;
```


**Returns**

[PlotEmptyCellsType](../plotemptycellstype/)

### setPlotEmptyCellsType(PlotEmptyCellsType) {#setPlotEmptyCellsType-plotemptycellstype-}

Gets and sets  how to plot the empty cells.

```javascript
setPlotEmptyCellsType(value: PlotEmptyCellsType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PlotEmptyCellsType](../plotemptycellstype/) | The value to set. |

### getPlotVisibleCellsOnly() {#getPlotVisibleCellsOnly--}

Indicates whether plot visible cells only.

```javascript
getPlotVisibleCellsOnly() : boolean;
```


### setPlotVisibleCellsOnly(boolean) {#setPlotVisibleCellsOnly-boolean-}

Indicates whether plot visible cells only.

```javascript
setPlotVisibleCellsOnly(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDisplayNaAsBlank() {#getDisplayNaAsBlank--}

Indicates whether displaying #N/A as blank value.

```javascript
getDisplayNaAsBlank() : boolean;
```


### setDisplayNaAsBlank(boolean) {#setDisplayNaAsBlank-boolean-}

Indicates whether displaying #N/A as blank value.

```javascript
setDisplayNaAsBlank(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getName() {#getName--}

Gets and sets the name of the chart.

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

Gets and sets the name of the chart.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getSizeWithWindow() {#getSizeWithWindow--}

True if Microsoft Excel resizes the chart to match the size of the chart sheet window.

```javascript
getSizeWithWindow() : boolean;
```


### setSizeWithWindow(boolean) {#setSizeWithWindow-boolean-}

True if Microsoft Excel resizes the chart to match the size of the chart sheet window.

```javascript
setSizeWithWindow(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getWorksheet() {#getWorksheet--}

Gets the worksheet which contains this chart.

```javascript
getWorksheet() : Worksheet;
```


**Returns**

[Worksheet](../worksheet/)

### getShapes() {#getShapes--}

Returns all drawing shapes in this chart.

```javascript
getShapes() : ShapeCollection;
```


**Returns**

[ShapeCollection](../shapecollection/)

### getPrintSize() {#getPrintSize--}

Gets and sets the printed chart size.

```javascript
getPrintSize() : PrintSizeType;
```


**Returns**

[PrintSizeType](../printsizetype/)

### setPrintSize(PrintSizeType) {#setPrintSize-printsizetype-}

Gets and sets the printed chart size.

```javascript
setPrintSize(value: PrintSizeType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PrintSizeType](../printsizetype/) | The value to set. |

### getType() {#getType--}

Gets or sets a chart's type.

```javascript
getType() : ChartType;
```


**Returns**

[ChartType](../charttype/)

### setType(ChartType) {#setType-charttype-}

Gets or sets a chart's type.

```javascript
setType(value: ChartType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ChartType](../charttype/) | The value to set. |

### getNSeries() {#getNSeries--}

Gets a [SeriesCollection](../seriescollection/) collection representing the data series in the chart.

```javascript
getNSeries() : SeriesCollection;
```


**Returns**

[SeriesCollection](../seriescollection/)

### getFilteredNSeries() {#getFilteredNSeries--}

Gets a [SeriesCollection](../seriescollection/) collection representing the data series that are filtered in the chart.

```javascript
getFilteredNSeries() : SeriesCollection;
```


**Returns**

[SeriesCollection](../seriescollection/)

### getTitle() {#getTitle--}

Gets the chart's title.

```javascript
getTitle() : Title;
```


**Returns**

[Title](../title/)

### getSubTitle() {#getSubTitle--}

Gets the chart's sub-title. Only for ODS format file.

```javascript
getSubTitle() : Title;
```


**Returns**

[Title](../title/)

### getPlotArea() {#getPlotArea--}

Gets the chart's plot area which includes axis tick labels.

```javascript
getPlotArea() : PlotArea;
```


**Returns**

[PlotArea](../plotarea/)

### getChartArea() {#getChartArea--}

Gets the chart area in the worksheet.

```javascript
getChartArea() : ChartArea;
```


**Returns**

[ChartArea](../chartarea/)

### getCategoryAxis() {#getCategoryAxis--}

Gets the chart's X axis.

```javascript
getCategoryAxis() : Axis;
```


**Returns**

[Axis](../axis/)

### getValueAxis() {#getValueAxis--}

Gets the chart's Y axis.

```javascript
getValueAxis() : Axis;
```


**Returns**

[Axis](../axis/)

### getSecondValueAxis() {#getSecondValueAxis--}

Gets the chart's second Y axis.

```javascript
getSecondValueAxis() : Axis;
```


**Returns**

[Axis](../axis/)

### getSecondCategoryAxis() {#getSecondCategoryAxis--}

Gets the chart's second X axis.

```javascript
getSecondCategoryAxis() : Axis;
```


**Returns**

[Axis](../axis/)

### getSeriesAxis() {#getSeriesAxis--}

Gets the chart's series axis.

```javascript
getSeriesAxis() : Axis;
```


**Returns**

[Axis](../axis/)

### getLegend() {#getLegend--}

Gets the chart legend.

```javascript
getLegend() : Legend;
```


**Returns**

[Legend](../legend/)

### getChartDataTable() {#getChartDataTable--}

Represents the chart data table.

```javascript
getChartDataTable() : ChartDataTable;
```


**Returns**

[ChartDataTable](../chartdatatable/)

### getShowLegend() {#getShowLegend--}

Gets or sets a value indicating whether the chart legend will be displayed. Default is true.

```javascript
getShowLegend() : boolean;
```


### setShowLegend(boolean) {#setShowLegend-boolean-}

Gets or sets a value indicating whether the chart legend will be displayed. Default is true.

```javascript
setShowLegend(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isRectangularCornered() {#isRectangularCornered--}

Gets or sets a value indicating whether the chart area is rectangular cornered. Default is true.

```javascript
isRectangularCornered() : boolean;
```


### setIsRectangularCornered(boolean) {#setIsRectangularCornered-boolean-}

Gets or sets a value indicating whether the chart area is rectangular cornered. Default is true.

```javascript
setIsRectangularCornered(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowDataTable() {#getShowDataTable--}

Gets or sets a value indicating whether the chart displays a data table.

```javascript
getShowDataTable() : boolean;
```


### setShowDataTable(boolean) {#setShowDataTable-boolean-}

Gets or sets a value indicating whether the chart displays a data table.

```javascript
setShowDataTable(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFirstSliceAngle() {#getFirstSliceAngle--}

Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.

```javascript
getFirstSliceAngle() : number;
```


### setFirstSliceAngle(number) {#setFirstSliceAngle-number-}

Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.

```javascript
setFirstSliceAngle(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getGapWidth() {#getGapWidth--}

Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500.

```javascript
getGapWidth() : number;
```


### setGapWidth(number) {#setGapWidth-number-}

Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500.

```javascript
setGapWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getGapDepth() {#getGapDepth--}

Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width. The value of this property must be between 0 and 500.

```javascript
getGapDepth() : number;
```


### setGapDepth(number) {#setGapDepth-number-}

Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width. The value of this property must be between 0 and 500.

```javascript
setGapDepth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getFloor() {#getFloor--}

Returns a [Floor](../floor/) object that represents the walls of a 3-D chart.

```javascript
getFloor() : Floor;
```


**Returns**

[Floor](../floor/)

**Remarks**

This property doesn't apply to 3-D pie charts.

### getWalls() {#getWalls--}

Returns a [Walls](../walls/) object that represents the walls of a 3-D chart.

```javascript
getWalls() : Walls;
```


**Returns**

[Walls](../walls/)

**Remarks**

This property doesn't apply to 3-D pie charts.

### getBackWall() {#getBackWall--}

Returns a [Walls](../walls/) object that represents the back wall of a 3-D chart.

```javascript
getBackWall() : Walls;
```


**Returns**

[Walls](../walls/)

### getSideWall() {#getSideWall--}

Returns a [Walls](../walls/) object that represents the side wall of a 3-D chart.

```javascript
getSideWall() : Walls;
```


**Returns**

[Walls](../walls/)

### getWallsAndGridlines2D() {#getWallsAndGridlines2D--}

True if gridlines are drawn two-dimensionally on a 3-D chart.

```javascript
getWallsAndGridlines2D() : boolean;
```


### setWallsAndGridlines2D(boolean) {#setWallsAndGridlines2D-boolean-}

True if gridlines are drawn two-dimensionally on a 3-D chart.

```javascript
setWallsAndGridlines2D(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRotationAngle() {#getRotationAngle--}

Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees).

```javascript
getRotationAngle() : number;
```


**Remarks**

The value of this property must be from 0 to 360, except for 3-D bar charts, where the value must be from 0 to 44. The default value is 20. Applies only to 3-D charts.

### setRotationAngle(number) {#setRotationAngle-number-}

Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees).

```javascript
setRotationAngle(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The value of this property must be from 0 to 360, except for 3-D bar charts, where the value must be from 0 to 44. The default value is 20. Applies only to 3-D charts.

### getElevation() {#getElevation--}

Represents the elevation of the 3-D chart view, in degrees.

```javascript
getElevation() : number;
```


**Remarks**

The chart elevation is the height at which you view the chart, in degrees. The default is 15 for most chart types. The value of this property must be between -90 and 90, except for 3-D bar charts, where it must be between 0 and 44.

### setElevation(number) {#setElevation-number-}

Represents the elevation of the 3-D chart view, in degrees.

```javascript
setElevation(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The chart elevation is the height at which you view the chart, in degrees. The default is 15 for most chart types. The value of this property must be between -90 and 90, except for 3-D bar charts, where it must be between 0 and 44.

### getRightAngleAxes() {#getRightAngleAxes--}

True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie Charts).

```javascript
getRightAngleAxes() : boolean;
```


**Remarks**

If this property is True, the Perspective property is ignored.

### setRightAngleAxes(boolean) {#setRightAngleAxes-boolean-}

True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie Charts).

```javascript
setRightAngleAxes(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

If this property is True, the Perspective property is ignored.

### getAutoScaling() {#getAutoScaling--}

True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. The RightAngleAxes property must be True.

```javascript
getAutoScaling() : boolean;
```


### setAutoScaling(boolean) {#setAutoScaling-boolean-}

True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. The RightAngleAxes property must be True.

```javascript
setAutoScaling(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHeightPercent() {#getHeightPercent--}

Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent).

```javascript
getHeightPercent() : number;
```


### setHeightPercent(number) {#setHeightPercent-number-}

Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent).

```javascript
setHeightPercent(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getPerspective() {#getPerspective--}

Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100. This property is ignored if the RightAngleAxes property is True.

```javascript
getPerspective() : number;
```


### setPerspective(number) {#setPerspective-number-}

Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100. This property is ignored if the RightAngleAxes property is True.

```javascript
setPerspective(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getIs3D() {#getIs3D--}

Indicates whether the chart is a 3d chart.

```javascript
getIs3D() : boolean;
```


### getDepthPercent() {#getDepthPercent--}

Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent).

```javascript
getDepthPercent() : number;
```


### setDepthPercent(number) {#setDepthPercent-number-}

Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent).

```javascript
setDepthPercent(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getPlacement() {#getPlacement--}

Represents the way the chart is attached to the cells below it.

```javascript
getPlacement() : PlacementType;
```


**Returns**

[PlacementType](../placementtype/)

### setPlacement(PlacementType) {#setPlacement-placementtype-}

Represents the way the chart is attached to the cells below it.

```javascript
setPlacement(value: PlacementType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PlacementType](../placementtype/) | The value to set. |

### getPageSetup() {#getPageSetup--}

Represents the page setup description in this chart.

```javascript
getPageSetup() : PageSetup;
```


**Returns**

[PageSetup](../pagesetup/)

### getLine() {#getLine--}

Gets the line.

```javascript
getLine() : Line;
```


**Returns**

[Line](../line/)

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

### changeTemplate(number[]) {#changeTemplate-numberarray-}

Change chart type with preset template.

```javascript
changeTemplate(data: number[]) : void;
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

<p>The format of the image is specified by using the extension of the file name. For example, if you specify "myfile.png", then the image will be saved in the PNG format. The following file extensions are recognized: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.</p> If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.

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

<p>The type of the image is specified by using <c>imageType</c>. The following types are supported: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.</p> If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.

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

If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.

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

<p>The type of the image is specified by using <c>imageType</c>. The following types are supported: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.</p> If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.

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

<p>The format of the image is specified by using the extension of the file name. For example, if you specify "myfile.png", then the image will be saved in the PNG format. The following file extensions are recognized: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.</p> If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. Please refer to <a href="http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html">Supported Charts List</a> for more details.

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

<p>The type of the image is specified by using <c>options.ImageType</c>. The following formats are supported: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.</p> If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. Please refer to <a href="http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html">Supported Charts List</a> for more details.

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


