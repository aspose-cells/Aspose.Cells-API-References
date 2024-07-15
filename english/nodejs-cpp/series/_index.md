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


## Methods

| Method | Description |
| --- | --- |
| [isFiltered()](#isFiltered--)| Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart. |
| [setIsFiltered(boolean)](#setIsFiltered-boolean-)| Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart. |
| [getLayoutProperties()](#getLayoutProperties--)| Represents the properties of layout. |
| [getPoints()](#getPoints--)| Gets the collection of points in a series in a chart. |
| [getArea()](#getArea--)| Represents the background area of Series object. |
| [getBorder()](#getBorder--)| Represents border of Series object. |
| [getName()](#getName--)| Gets or sets the name of the data series. |
| [setName(string)](#setName-string-)| Gets or sets the name of the data series. |
| [getDisplayName()](#getDisplayName--)| Gets the series's name that displays on the chart graph. |
| [getCountOfDataValues()](#getCountOfDataValues--)| Gets the number of the data values. |
| [isVerticalValues()](#isVerticalValues--)| Indicates whether the data source is vertical. |
| [getValues()](#getValues--)| Represents the Y values of this chart series. |
| [setValues(string)](#setValues-string-)| Represents the Y values of this chart series. |
| [getValuesFormatCode()](#getValuesFormatCode--)| Represents format code of Values's NumberList. |
| [setValuesFormatCode(string)](#setValuesFormatCode-string-)| Represents format code of Values's NumberList. |
| [getXValuesFormatCode()](#getXValuesFormatCode--)| Represents format code of X Values's NumberList. |
| [setXValuesFormatCode(string)](#setXValuesFormatCode-string-)| Represents format code of X Values's NumberList. |
| [getXValues()](#getXValues--)| Represents the x values of the chart series. |
| [setXValues(string)](#setXValues-string-)| Represents the x values of the chart series. |
| [getBubbleSizes()](#getBubbleSizes--)| Gets or sets the bubble sizes values of the chart series. |
| [setBubbleSizes(string)](#setBubbleSizes-string-)| Gets or sets the bubble sizes values of the chart series. |
| [getTrendLines()](#getTrendLines--)| Returns all the trendlines of this series. |
| [getSmooth()](#getSmooth--)| Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line and scatter connected by lines charts. |
| [setSmooth(boolean)](#setSmooth-boolean-)| Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line and scatter connected by lines charts. |
| [getShadow()](#getShadow--)| True if the series has a shadow. |
| [setShadow(boolean)](#setShadow-boolean-)| True if the series has a shadow. |
| [getHas3DEffect()](#getHas3DEffect--)| True if the series has a three-dimensional appearance. Applies only to bubble charts. |
| [setHas3DEffect(boolean)](#setHas3DEffect-boolean-)| True if the series has a three-dimensional appearance. Applies only to bubble charts. |
| [getBar3DShapeType()](#getBar3DShapeType--)| Gets or sets the 3D shape type used with the 3-D bar or column chart. |
| [setBar3DShapeType(Bar3DShapeType)](#setBar3DShapeType-bar3dshapetype-)| Gets or sets the 3D shape type used with the 3-D bar or column chart. |
| [getDataLabels()](#getDataLabels--)| Represents the DataLabels object for the specified ASeries. |
| [getType()](#getType--)| Gets or sets a data series' type. |
| [setType(ChartType)](#setType-charttype-)| Gets or sets a data series' type. |
| [getMarker()](#getMarker--)| Gets the <see cref="Marker">marker</see>. |
| [getPlotOnSecondAxis()](#getPlotOnSecondAxis--)| Indicates if this series is plotted on second value axis. |
| [setPlotOnSecondAxis(boolean)](#setPlotOnSecondAxis-boolean-)| Indicates if this series is plotted on second value axis. |
| [getXErrorBar()](#getXErrorBar--)| Represents X direction error bar of the series. |
| [getYErrorBar()](#getYErrorBar--)| Represents Y direction error bar of the series. |
| [getHasHiLoLines()](#getHasHiLoLines--)| True if the line chart has high-low lines. Applies only to line charts. |
| [setHasHiLoLines(boolean)](#setHasHiLoLines-boolean-)| True if the line chart has high-low lines. Applies only to line charts. |
| [getHiLoLines()](#getHiLoLines--)| Returns a HiLoLines object that represents the high-low lines for a series on a line chart. Applies only to line charts. |
| [getHasSeriesLines()](#getHasSeriesLines--)| True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts. |
| [setHasSeriesLines(boolean)](#setHasSeriesLines-boolean-)| True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts. |
| [getSeriesLines()](#getSeriesLines--)| Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. Applies only to stacked bar and stacked column charts. |
| [getHasDropLines()](#getHasDropLines--)| True if the chart has drop lines. Applies only to line chart or area charts. |
| [setHasDropLines(boolean)](#setHasDropLines-boolean-)| True if the chart has drop lines. Applies only to line chart or area charts. |
| [getDropLines()](#getDropLines--)| Returns a [Line](../line/) object that represents the drop lines for a series on the line chart or area chart. Applies only to line chart or area charts. |
| [getHasUpDownBars()](#getHasUpDownBars--)| True if a line chart has up and down bars. Applies only to line charts. |
| [setHasUpDownBars(boolean)](#setHasUpDownBars-boolean-)| True if a line chart has up and down bars. Applies only to line charts. |
| [getUpBars()](#getUpBars--)| Returns an DropBars object that represents the up bars on a line chart. Applies only to line charts. |
| [getDownBars()](#getDownBars--)| Returns a [DropBars](../dropbars/) object that represents the down bars on a line chart. Applies only to line charts. |
| [isColorVaried()](#isColorVaried--)| Represents if the color of points is varied. The chart must contain only one series. |
| [setIsColorVaried(boolean)](#setIsColorVaried-boolean-)| Represents if the color of points is varied. The chart must contain only one series. |
| [getGapWidth()](#getGapWidth--)| Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500. |
| [setGapWidth(number)](#setGapWidth-number-)| Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500. |
| [getFirstSliceAngle()](#getFirstSliceAngle--)| Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360. |
| [setFirstSliceAngle(number)](#setFirstSliceAngle-number-)| Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360. |
| [getOverlap()](#getOverlap--)| Specifies how bars and columns are positioned. Can be a value between – 100 and 100. Applies only to 2-D bar and 2-D column charts. |
| [setOverlap(number)](#setOverlap-number-)| Specifies how bars and columns are positioned. Can be a value between – 100 and 100. Applies only to 2-D bar and 2-D column charts. |
| [getSecondPlotSize()](#getSecondPlotSize--)| Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of the size of the primary pie. Can be a value from 5 to 200. |
| [setSecondPlotSize(number)](#setSecondPlotSize-number-)| Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of the size of the primary pie. Can be a value from 5 to 200. |
| [getSplitType()](#getSplitType--)| Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. |
| [setSplitType(ChartSplitType)](#setSplitType-chartsplittype-)| Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. |
| [getSplitValue()](#getSplitValue--)| Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. |
| [setSplitValue(number)](#setSplitValue-number-)| Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. |
| [isAutoSplit()](#isAutoSplit--)| Indicates whether the threshold value is automatic. |
| [getBubbleScale()](#getBubbleScale--)| Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, corresponding to a percentage of the default size. Applies only to bubble charts. |
| [setBubbleScale(number)](#setBubbleScale-number-)| Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, corresponding to a percentage of the default size. Applies only to bubble charts. |
| [getSizeRepresents()](#getSizeRepresents--)| Gets or sets what the bubble size represents on a bubble chart. |
| [setSizeRepresents(BubbleSizeRepresents)](#setSizeRepresents-bubblesizerepresents-)| Gets or sets what the bubble size represents on a bubble chart. |
| [getShowNegativeBubbles()](#getShowNegativeBubbles--)| True if negative bubbles are shown for the chart group. Valid only for bubble charts. |
| [setShowNegativeBubbles(boolean)](#setShowNegativeBubbles-boolean-)| True if negative bubbles are shown for the chart group. Valid only for bubble charts. |
| [getDoughnutHoleSize()](#getDoughnutHoleSize--)| Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart size, between 10 and 90 percent. |
| [setDoughnutHoleSize(number)](#setDoughnutHoleSize-number-)| Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart size, between 10 and 90 percent. |
| [getExplosion()](#getExplosion--)| The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [setExplosion(number)](#setExplosion-number-)| The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [getHasRadarAxisLabels()](#getHasRadarAxisLabels--)| True if a radar chart has category axis labels. Applies only to radar charts. |
| [setHasRadarAxisLabels(boolean)](#setHasRadarAxisLabels-boolean-)| True if a radar chart has category axis labels. Applies only to radar charts. |
| [getHasLeaderLines()](#getHasLeaderLines--)| True if the series has leader lines. |
| [setHasLeaderLines(boolean)](#setHasLeaderLines-boolean-)| True if the series has leader lines. |
| [getLeaderLines()](#getLeaderLines--)| Represents leader lines on a chart. Leader lines connect data labels to data points. This object isn’t a collection; there’s no object that represents a single leader line. |
| [getLegendEntry()](#getLegendEntry--)| Gets the legend entry according to this series. |
| [getShapeProperties()](#getShapeProperties--)| Gets the [ShapePropertyCollection](../shapepropertycollection/) object that holds the visual shape properties of the Series. |
| [move(number)](#move-number-)| Moves the series up or down. |


### isFiltered() {#isFiltered--}

Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart.

```javascript
isFiltered() : boolean;
```


### setIsFiltered(boolean) {#setIsFiltered-boolean-}

Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart.

```javascript
setIsFiltered(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getLayoutProperties() {#getLayoutProperties--}

Represents the properties of layout.

```javascript
getLayoutProperties() : SeriesLayoutProperties;
```


**Returns**

[SeriesLayoutProperties](../serieslayoutproperties/)

### getPoints() {#getPoints--}

Gets the collection of points in a series in a chart.

```javascript
getPoints() : ChartPointCollection;
```


**Returns**

[ChartPointCollection](../chartpointcollection/)

**Remarks**

When the chart is Pie of Pie or Bar of Pie, the last point is other point in first pie plot.

### getArea() {#getArea--}

Represents the background area of Series object.

```javascript
getArea() : Area;
```


**Returns**

[Area](../area/)

### getBorder() {#getBorder--}

Represents border of Series object.

```javascript
getBorder() : Line;
```


**Returns**

[Line](../line/)

### getName() {#getName--}

Gets or sets the name of the data series.

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

Gets or sets the name of the data series.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getDisplayName() {#getDisplayName--}

Gets the series's name that displays on the chart graph.

```javascript
getDisplayName() : string;
```


### getCountOfDataValues() {#getCountOfDataValues--}

Gets the number of the data values.

```javascript
getCountOfDataValues() : number;
```


### isVerticalValues() {#isVerticalValues--}

Indicates whether the data source is vertical.

```javascript
isVerticalValues() : boolean;
```


### getValues() {#getValues--}

Represents the Y values of this chart series.

```javascript
getValues() : string;
```


### setValues(string) {#setValues-string-}

Represents the Y values of this chart series.

```javascript
setValues(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getValuesFormatCode() {#getValuesFormatCode--}

Represents format code of Values's NumberList.

```javascript
getValuesFormatCode() : string;
```


### setValuesFormatCode(string) {#setValuesFormatCode-string-}

Represents format code of Values's NumberList.

```javascript
setValuesFormatCode(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getXValuesFormatCode() {#getXValuesFormatCode--}

Represents format code of X Values's NumberList.

```javascript
getXValuesFormatCode() : string;
```


### setXValuesFormatCode(string) {#setXValuesFormatCode-string-}

Represents format code of X Values's NumberList.

```javascript
setXValuesFormatCode(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getXValues() {#getXValues--}

Represents the x values of the chart series.

```javascript
getXValues() : string;
```


### setXValues(string) {#setXValues-string-}

Represents the x values of the chart series.

```javascript
setXValues(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getBubbleSizes() {#getBubbleSizes--}

Gets or sets the bubble sizes values of the chart series.

```javascript
getBubbleSizes() : string;
```


### setBubbleSizes(string) {#setBubbleSizes-string-}

Gets or sets the bubble sizes values of the chart series.

```javascript
setBubbleSizes(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getTrendLines() {#getTrendLines--}

Returns all the trendlines of this series.

```javascript
getTrendLines() : TrendlineCollection;
```


**Returns**

[TrendlineCollection](../trendlinecollection/)

### getSmooth() {#getSmooth--}

Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line and scatter connected by lines charts.

```javascript
getSmooth() : boolean;
```


### setSmooth(boolean) {#setSmooth-boolean-}

Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line and scatter connected by lines charts.

```javascript
setSmooth(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShadow() {#getShadow--}

True if the series has a shadow.

```javascript
getShadow() : boolean;
```


### setShadow(boolean) {#setShadow-boolean-}

True if the series has a shadow.

```javascript
setShadow(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHas3DEffect() {#getHas3DEffect--}

True if the series has a three-dimensional appearance. Applies only to bubble charts.

```javascript
getHas3DEffect() : boolean;
```


### setHas3DEffect(boolean) {#setHas3DEffect-boolean-}

True if the series has a three-dimensional appearance. Applies only to bubble charts.

```javascript
setHas3DEffect(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getBar3DShapeType() {#getBar3DShapeType--}

Gets or sets the 3D shape type used with the 3-D bar or column chart.

```javascript
getBar3DShapeType() : Bar3DShapeType;
```


**Returns**

[Bar3DShapeType](../bar3dshapetype/)

### setBar3DShapeType(Bar3DShapeType) {#setBar3DShapeType-bar3dshapetype-}

Gets or sets the 3D shape type used with the 3-D bar or column chart.

```javascript
setBar3DShapeType(value: Bar3DShapeType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Bar3DShapeType](../bar3dshapetype/) | The value to set. |

### getDataLabels() {#getDataLabels--}

Represents the DataLabels object for the specified ASeries.

```javascript
getDataLabels() : DataLabels;
```


**Returns**

[DataLabels](../datalabels/)

### getType() {#getType--}

Gets or sets a data series' type.

```javascript
getType() : ChartType;
```


**Returns**

[ChartType](../charttype/)

### setType(ChartType) {#setType-charttype-}

Gets or sets a data series' type.

```javascript
setType(value: ChartType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ChartType](../charttype/) | The value to set. |

### getMarker() {#getMarker--}

Gets the <see cref="Marker">marker</see>.

```javascript
getMarker() : Marker;
```


**Returns**

[Marker](../marker/)

### getPlotOnSecondAxis() {#getPlotOnSecondAxis--}

Indicates if this series is plotted on second value axis.

```javascript
getPlotOnSecondAxis() : boolean;
```


### setPlotOnSecondAxis(boolean) {#setPlotOnSecondAxis-boolean-}

Indicates if this series is plotted on second value axis.

```javascript
setPlotOnSecondAxis(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getXErrorBar() {#getXErrorBar--}

Represents X direction error bar of the series.

```javascript
getXErrorBar() : ErrorBar;
```


**Returns**

[ErrorBar](../errorbar/)

### getYErrorBar() {#getYErrorBar--}

Represents Y direction error bar of the series.

```javascript
getYErrorBar() : ErrorBar;
```


**Returns**

[ErrorBar](../errorbar/)

### getHasHiLoLines() {#getHasHiLoLines--}

True if the line chart has high-low lines. Applies only to line charts.

```javascript
getHasHiLoLines() : boolean;
```


### setHasHiLoLines(boolean) {#setHasHiLoLines-boolean-}

True if the line chart has high-low lines. Applies only to line charts.

```javascript
setHasHiLoLines(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHiLoLines() {#getHiLoLines--}

Returns a HiLoLines object that represents the high-low lines for a series on a line chart. Applies only to line charts.

```javascript
getHiLoLines() : Line;
```


**Returns**

[Line](../line/)

### getHasSeriesLines() {#getHasSeriesLines--}

True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts.

```javascript
getHasSeriesLines() : boolean;
```


### setHasSeriesLines(boolean) {#setHasSeriesLines-boolean-}

True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts.

```javascript
setHasSeriesLines(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSeriesLines() {#getSeriesLines--}

Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. Applies only to stacked bar and stacked column charts.

```javascript
getSeriesLines() : Line;
```


**Returns**

[Line](../line/)

### getHasDropLines() {#getHasDropLines--}

True if the chart has drop lines. Applies only to line chart or area charts.

```javascript
getHasDropLines() : boolean;
```


### setHasDropLines(boolean) {#setHasDropLines-boolean-}

True if the chart has drop lines. Applies only to line chart or area charts.

```javascript
setHasDropLines(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDropLines() {#getDropLines--}

Returns a [Line](../line/) object that represents the drop lines for a series on the line chart or area chart. Applies only to line chart or area charts.

```javascript
getDropLines() : Line;
```


**Returns**

[Line](../line/)

### getHasUpDownBars() {#getHasUpDownBars--}

True if a line chart has up and down bars. Applies only to line charts.

```javascript
getHasUpDownBars() : boolean;
```


### setHasUpDownBars(boolean) {#setHasUpDownBars-boolean-}

True if a line chart has up and down bars. Applies only to line charts.

```javascript
setHasUpDownBars(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getUpBars() {#getUpBars--}

Returns an DropBars object that represents the up bars on a line chart. Applies only to line charts.

```javascript
getUpBars() : DropBars;
```


**Returns**

[DropBars](../dropbars/)

### getDownBars() {#getDownBars--}

Returns a [DropBars](../dropbars/) object that represents the down bars on a line chart. Applies only to line charts.

```javascript
getDownBars() : DropBars;
```


**Returns**

[DropBars](../dropbars/)

### isColorVaried() {#isColorVaried--}

Represents if the color of points is varied. The chart must contain only one series.

```javascript
isColorVaried() : boolean;
```


### setIsColorVaried(boolean) {#setIsColorVaried-boolean-}

Represents if the color of points is varied. The chart must contain only one series.

```javascript
setIsColorVaried(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

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

### getOverlap() {#getOverlap--}

Specifies how bars and columns are positioned. Can be a value between – 100 and 100. Applies only to 2-D bar and 2-D column charts.

```javascript
getOverlap() : number;
```


### setOverlap(number) {#setOverlap-number-}

Specifies how bars and columns are positioned. Can be a value between – 100 and 100. Applies only to 2-D bar and 2-D column charts.

```javascript
setOverlap(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getSecondPlotSize() {#getSecondPlotSize--}

Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of the size of the primary pie. Can be a value from 5 to 200.

```javascript
getSecondPlotSize() : number;
```


### setSecondPlotSize(number) {#setSecondPlotSize-number-}

Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of the size of the primary pie. Can be a value from 5 to 200.

```javascript
setSecondPlotSize(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getSplitType() {#getSplitType--}

Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.

```javascript
getSplitType() : ChartSplitType;
```


**Returns**

[ChartSplitType](../chartsplittype/)

### setSplitType(ChartSplitType) {#setSplitType-chartsplittype-}

Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.

```javascript
setSplitType(value: ChartSplitType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ChartSplitType](../chartsplittype/) | The value to set. |

### getSplitValue() {#getSplitValue--}

Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.

```javascript
getSplitValue() : number;
```


### setSplitValue(number) {#setSplitValue-number-}

Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.

```javascript
setSplitValue(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isAutoSplit() {#isAutoSplit--}

Indicates whether the threshold value is automatic.

```javascript
isAutoSplit() : boolean;
```


### getBubbleScale() {#getBubbleScale--}

Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, corresponding to a percentage of the default size. Applies only to bubble charts.

```javascript
getBubbleScale() : number;
```


### setBubbleScale(number) {#setBubbleScale-number-}

Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, corresponding to a percentage of the default size. Applies only to bubble charts.

```javascript
setBubbleScale(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getSizeRepresents() {#getSizeRepresents--}

Gets or sets what the bubble size represents on a bubble chart.

```javascript
getSizeRepresents() : BubbleSizeRepresents;
```


**Returns**

[BubbleSizeRepresents](../bubblesizerepresents/)

**Remarks**

BubbleSizeRepresents.SizeIsArea means the value [Series.BubbleSizes](../series.bubblesizes/) is the area of the bubble. BubbleSizeRepresents.SizeIsWidth means the value [Series.BubbleSizes](../series.bubblesizes/) is the width of the bubble.

### setSizeRepresents(BubbleSizeRepresents) {#setSizeRepresents-bubblesizerepresents-}

Gets or sets what the bubble size represents on a bubble chart.

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

True if negative bubbles are shown for the chart group. Valid only for bubble charts.

```javascript
getShowNegativeBubbles() : boolean;
```


### setShowNegativeBubbles(boolean) {#setShowNegativeBubbles-boolean-}

True if negative bubbles are shown for the chart group. Valid only for bubble charts.

```javascript
setShowNegativeBubbles(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDoughnutHoleSize() {#getDoughnutHoleSize--}

Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart size, between 10 and 90 percent.

```javascript
getDoughnutHoleSize() : number;
```


### setDoughnutHoleSize(number) {#setDoughnutHoleSize-number-}

Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart size, between 10 and 90 percent.

```javascript
setDoughnutHoleSize(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getExplosion() {#getExplosion--}

The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.

```javascript
getExplosion() : number;
```


### setExplosion(number) {#setExplosion-number-}

The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.

```javascript
setExplosion(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHasRadarAxisLabels() {#getHasRadarAxisLabels--}

True if a radar chart has category axis labels. Applies only to radar charts.

```javascript
getHasRadarAxisLabels() : boolean;
```


### setHasRadarAxisLabels(boolean) {#setHasRadarAxisLabels-boolean-}

True if a radar chart has category axis labels. Applies only to radar charts.

```javascript
setHasRadarAxisLabels(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHasLeaderLines() {#getHasLeaderLines--}

True if the series has leader lines.

```javascript
getHasLeaderLines() : boolean;
```


### setHasLeaderLines(boolean) {#setHasLeaderLines-boolean-}

True if the series has leader lines.

```javascript
setHasLeaderLines(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getLeaderLines() {#getLeaderLines--}

Represents leader lines on a chart. Leader lines connect data labels to data points. This object isn’t a collection; there’s no object that represents a single leader line.

```javascript
getLeaderLines() : Line;
```


**Returns**

[Line](../line/)

### getLegendEntry() {#getLegendEntry--}

Gets the legend entry according to this series.

```javascript
getLegendEntry() : LegendEntry;
```


**Returns**

[LegendEntry](../legendentry/)

### getShapeProperties() {#getShapeProperties--}

Gets the [ShapePropertyCollection](../shapepropertycollection/) object that holds the visual shape properties of the Series.

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


