---
title: SparklineGroup
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Sparkline..sparkline is organized into sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type display settings and axis settings for the sparklines.
type: docs
url: /nodejs-cpp/sparklinegroup/
---

## SparklineGroup class

[Sparkline](../sparkline/) is organized into sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type, display settings and axis settings for the sparklines.

```javascript
class SparklineGroup;
```


## Properties

| Property | Type | Description |
| --- | --- | --- |
| [presetStyle](#presetStyle--)| SparklinePresetStyleType | Gets and sets the preset style type of the sparkline group. |
| [sparklines](#sparklines--)| SparklineCollection | Readonly. Gets the collection of [Sparkline](../sparkline/) object. |
| [type](#type--)| SparklineType | Indicates the sparkline type of the sparkline group. |
| [plotEmptyCellsType](#plotEmptyCellsType--)| PlotEmptyCellsType | Indicates how to plot empty cells. |
| [displayHidden](#displayHidden--)| boolean | Indicates whether to show data in hidden rows and columns. |
| [showHighPoint](#showHighPoint--)| boolean | Indicates whether to highlight the highest points of data in the sparkline group. |
| [highPointColor](#highPointColor--)| CellsColor | Gets and sets the color of the highest points of data in the sparkline group. |
| [showLowPoint](#showLowPoint--)| boolean | Indicates whether to highlight the lowest points of data in the sparkline group. |
| [lowPointColor](#lowPointColor--)| CellsColor | Gets and sets the color of the lowest points of data in the sparkline group. |
| [showNegativePoints](#showNegativePoints--)| boolean | Indicates whether to highlight the negative values on the sparkline group with a different color or marker. |
| [negativePointsColor](#negativePointsColor--)| CellsColor | Gets and sets the color of the negative values on the sparkline group. |
| [showFirstPoint](#showFirstPoint--)| boolean | Indicates whether to highlight the first point of data in the sparkline group. |
| [firstPointColor](#firstPointColor--)| CellsColor | Gets and sets the color of the first point of data in the sparkline group. |
| [showLastPoint](#showLastPoint--)| boolean | Indicates whether to highlight the last point of data in the sparkline group. |
| [lastPointColor](#lastPointColor--)| CellsColor | Gets and sets the color of the last point of data in the sparkline group. |
| [showMarkers](#showMarkers--)| boolean | Indicates whether to highlight each point in each line sparkline in the sparkline group. |
| [markersColor](#markersColor--)| CellsColor | Gets and sets the color of points in each line sparkline in the sparkline group. |
| [seriesColor](#seriesColor--)| CellsColor | Gets and sets the color of the sparklines in the sparkline group. |
| [plotRightToLeft](#plotRightToLeft--)| boolean | Indicates whether the plot data is right to left. |
| [lineWeight](#lineWeight--)| number | Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points. |
| [horizontalAxisColor](#horizontalAxisColor--)| CellsColor | Gets and sets the color of the horizontal axis in the sparkline group. |
| [showHorizontalAxis](#showHorizontalAxis--)| boolean | Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that crosses the zero axis. |
| [horizontalAxisDateRange](#horizontalAxisDateRange--)| string | Represents the range that contains the date values for the sparkline data. |
| [verticalAxisMaxValueType](#verticalAxisMaxValueType--)| SparklineAxisMinMaxType | Represents the vertical axis maximum value type. |
| [verticalAxisMaxValue](#verticalAxisMaxValue--)| number | Gets and sets the custom maximum value for the vertical axis. |
| [verticalAxisMinValueType](#verticalAxisMinValueType--)| SparklineAxisMinMaxType | Represents the vertical axis minimum value type. |
| [verticalAxisMinValue](#verticalAxisMinValue--)| number | Gets and sets the custom minimum value for the vertical axis. |

## Methods

| Method | Description |
| --- | --- |
| [getPresetStyle()](#getPresetStyle--)| <b>@deprecated.</b> Please use the 'presetStyle' property instead. Gets and sets the preset style type of the sparkline group. |
| [setPresetStyle(SparklinePresetStyleType)](#setPresetStyle-sparklinepresetstyletype-)| <b>@deprecated.</b> Please use the 'presetStyle' property instead. Gets and sets the preset style type of the sparkline group. |
| [getSparklines()](#getSparklines--)| <b>@deprecated.</b> Please use the 'sparklines' property instead. Gets the collection of [Sparkline](../sparkline/) object. |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Indicates the sparkline type of the sparkline group. |
| [setType(SparklineType)](#setType-sparklinetype-)| <b>@deprecated.</b> Please use the 'type' property instead. Indicates the sparkline type of the sparkline group. |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--)| <b>@deprecated.</b> Please use the 'plotEmptyCellsType' property instead. Indicates how to plot empty cells. |
| [setPlotEmptyCellsType(PlotEmptyCellsType)](#setPlotEmptyCellsType-plotemptycellstype-)| <b>@deprecated.</b> Please use the 'plotEmptyCellsType' property instead. Indicates how to plot empty cells. |
| [getDisplayHidden()](#getDisplayHidden--)| <b>@deprecated.</b> Please use the 'displayHidden' property instead. Indicates whether to show data in hidden rows and columns. |
| [setDisplayHidden(boolean)](#setDisplayHidden-boolean-)| <b>@deprecated.</b> Please use the 'displayHidden' property instead. Indicates whether to show data in hidden rows and columns. |
| [getShowHighPoint()](#getShowHighPoint--)| <b>@deprecated.</b> Please use the 'showHighPoint' property instead. Indicates whether to highlight the highest points of data in the sparkline group. |
| [setShowHighPoint(boolean)](#setShowHighPoint-boolean-)| <b>@deprecated.</b> Please use the 'showHighPoint' property instead. Indicates whether to highlight the highest points of data in the sparkline group. |
| [getHighPointColor()](#getHighPointColor--)| <b>@deprecated.</b> Please use the 'highPointColor' property instead. Gets and sets the color of the highest points of data in the sparkline group. |
| [setHighPointColor(CellsColor)](#setHighPointColor-cellscolor-)| <b>@deprecated.</b> Please use the 'highPointColor' property instead. Gets and sets the color of the highest points of data in the sparkline group. |
| [getShowLowPoint()](#getShowLowPoint--)| <b>@deprecated.</b> Please use the 'showLowPoint' property instead. Indicates whether to highlight the lowest points of data in the sparkline group. |
| [setShowLowPoint(boolean)](#setShowLowPoint-boolean-)| <b>@deprecated.</b> Please use the 'showLowPoint' property instead. Indicates whether to highlight the lowest points of data in the sparkline group. |
| [getLowPointColor()](#getLowPointColor--)| <b>@deprecated.</b> Please use the 'lowPointColor' property instead. Gets and sets the color of the lowest points of data in the sparkline group. |
| [setLowPointColor(CellsColor)](#setLowPointColor-cellscolor-)| <b>@deprecated.</b> Please use the 'lowPointColor' property instead. Gets and sets the color of the lowest points of data in the sparkline group. |
| [getShowNegativePoints()](#getShowNegativePoints--)| <b>@deprecated.</b> Please use the 'showNegativePoints' property instead. Indicates whether to highlight the negative values on the sparkline group with a different color or marker. |
| [setShowNegativePoints(boolean)](#setShowNegativePoints-boolean-)| <b>@deprecated.</b> Please use the 'showNegativePoints' property instead. Indicates whether to highlight the negative values on the sparkline group with a different color or marker. |
| [getNegativePointsColor()](#getNegativePointsColor--)| <b>@deprecated.</b> Please use the 'negativePointsColor' property instead. Gets and sets the color of the negative values on the sparkline group. |
| [setNegativePointsColor(CellsColor)](#setNegativePointsColor-cellscolor-)| <b>@deprecated.</b> Please use the 'negativePointsColor' property instead. Gets and sets the color of the negative values on the sparkline group. |
| [getShowFirstPoint()](#getShowFirstPoint--)| <b>@deprecated.</b> Please use the 'showFirstPoint' property instead. Indicates whether to highlight the first point of data in the sparkline group. |
| [setShowFirstPoint(boolean)](#setShowFirstPoint-boolean-)| <b>@deprecated.</b> Please use the 'showFirstPoint' property instead. Indicates whether to highlight the first point of data in the sparkline group. |
| [getFirstPointColor()](#getFirstPointColor--)| <b>@deprecated.</b> Please use the 'firstPointColor' property instead. Gets and sets the color of the first point of data in the sparkline group. |
| [setFirstPointColor(CellsColor)](#setFirstPointColor-cellscolor-)| <b>@deprecated.</b> Please use the 'firstPointColor' property instead. Gets and sets the color of the first point of data in the sparkline group. |
| [getShowLastPoint()](#getShowLastPoint--)| <b>@deprecated.</b> Please use the 'showLastPoint' property instead. Indicates whether to highlight the last point of data in the sparkline group. |
| [setShowLastPoint(boolean)](#setShowLastPoint-boolean-)| <b>@deprecated.</b> Please use the 'showLastPoint' property instead. Indicates whether to highlight the last point of data in the sparkline group. |
| [getLastPointColor()](#getLastPointColor--)| <b>@deprecated.</b> Please use the 'lastPointColor' property instead. Gets and sets the color of the last point of data in the sparkline group. |
| [setLastPointColor(CellsColor)](#setLastPointColor-cellscolor-)| <b>@deprecated.</b> Please use the 'lastPointColor' property instead. Gets and sets the color of the last point of data in the sparkline group. |
| [getShowMarkers()](#getShowMarkers--)| <b>@deprecated.</b> Please use the 'showMarkers' property instead. Indicates whether to highlight each point in each line sparkline in the sparkline group. |
| [setShowMarkers(boolean)](#setShowMarkers-boolean-)| <b>@deprecated.</b> Please use the 'showMarkers' property instead. Indicates whether to highlight each point in each line sparkline in the sparkline group. |
| [getMarkersColor()](#getMarkersColor--)| <b>@deprecated.</b> Please use the 'markersColor' property instead. Gets and sets the color of points in each line sparkline in the sparkline group. |
| [setMarkersColor(CellsColor)](#setMarkersColor-cellscolor-)| <b>@deprecated.</b> Please use the 'markersColor' property instead. Gets and sets the color of points in each line sparkline in the sparkline group. |
| [getSeriesColor()](#getSeriesColor--)| <b>@deprecated.</b> Please use the 'seriesColor' property instead. Gets and sets the color of the sparklines in the sparkline group. |
| [setSeriesColor(CellsColor)](#setSeriesColor-cellscolor-)| <b>@deprecated.</b> Please use the 'seriesColor' property instead. Gets and sets the color of the sparklines in the sparkline group. |
| [getPlotRightToLeft()](#getPlotRightToLeft--)| <b>@deprecated.</b> Please use the 'plotRightToLeft' property instead. Indicates whether the plot data is right to left. |
| [setPlotRightToLeft(boolean)](#setPlotRightToLeft-boolean-)| <b>@deprecated.</b> Please use the 'plotRightToLeft' property instead. Indicates whether the plot data is right to left. |
| [getLineWeight()](#getLineWeight--)| <b>@deprecated.</b> Please use the 'lineWeight' property instead. Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points. |
| [setLineWeight(number)](#setLineWeight-number-)| <b>@deprecated.</b> Please use the 'lineWeight' property instead. Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points. |
| [getHorizontalAxisColor()](#getHorizontalAxisColor--)| <b>@deprecated.</b> Please use the 'horizontalAxisColor' property instead. Gets and sets the color of the horizontal axis in the sparkline group. |
| [setHorizontalAxisColor(CellsColor)](#setHorizontalAxisColor-cellscolor-)| <b>@deprecated.</b> Please use the 'horizontalAxisColor' property instead. Gets and sets the color of the horizontal axis in the sparkline group. |
| [getShowHorizontalAxis()](#getShowHorizontalAxis--)| <b>@deprecated.</b> Please use the 'showHorizontalAxis' property instead. Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that crosses the zero axis. |
| [setShowHorizontalAxis(boolean)](#setShowHorizontalAxis-boolean-)| <b>@deprecated.</b> Please use the 'showHorizontalAxis' property instead. Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that crosses the zero axis. |
| [getHorizontalAxisDateRange()](#getHorizontalAxisDateRange--)| <b>@deprecated.</b> Please use the 'horizontalAxisDateRange' property instead. Represents the range that contains the date values for the sparkline data. |
| [setHorizontalAxisDateRange(string)](#setHorizontalAxisDateRange-string-)| <b>@deprecated.</b> Please use the 'horizontalAxisDateRange' property instead. Represents the range that contains the date values for the sparkline data. |
| [getVerticalAxisMaxValueType()](#getVerticalAxisMaxValueType--)| <b>@deprecated.</b> Please use the 'verticalAxisMaxValueType' property instead. Represents the vertical axis maximum value type. |
| [setVerticalAxisMaxValueType(SparklineAxisMinMaxType)](#setVerticalAxisMaxValueType-sparklineaxisminmaxtype-)| <b>@deprecated.</b> Please use the 'verticalAxisMaxValueType' property instead. Represents the vertical axis maximum value type. |
| [getVerticalAxisMaxValue()](#getVerticalAxisMaxValue--)| <b>@deprecated.</b> Please use the 'verticalAxisMaxValue' property instead. Gets and sets the custom maximum value for the vertical axis. |
| [setVerticalAxisMaxValue(number)](#setVerticalAxisMaxValue-number-)| <b>@deprecated.</b> Please use the 'verticalAxisMaxValue' property instead. Gets and sets the custom maximum value for the vertical axis. |
| [getVerticalAxisMinValueType()](#getVerticalAxisMinValueType--)| <b>@deprecated.</b> Please use the 'verticalAxisMinValueType' property instead. Represents the vertical axis minimum value type. |
| [setVerticalAxisMinValueType(SparklineAxisMinMaxType)](#setVerticalAxisMinValueType-sparklineaxisminmaxtype-)| <b>@deprecated.</b> Please use the 'verticalAxisMinValueType' property instead. Represents the vertical axis minimum value type. |
| [getVerticalAxisMinValue()](#getVerticalAxisMinValue--)| <b>@deprecated.</b> Please use the 'verticalAxisMinValue' property instead. Gets and sets the custom minimum value for the vertical axis. |
| [setVerticalAxisMinValue(number)](#setVerticalAxisMinValue-number-)| <b>@deprecated.</b> Please use the 'verticalAxisMinValue' property instead. Gets and sets the custom minimum value for the vertical axis. |
| [resetRanges(string, boolean, CellArea)](#resetRanges-string-boolean-cellarea-)| Resets the data range and location range of the sparkline group. This method will clear original sparkline items in the group and creates new sparkline items for the new ranges. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### presetStyle {#presetStyle--}

Gets and sets the preset style type of the sparkline group.

```javascript
presetStyle : SparklinePresetStyleType;
```


### sparklines {#sparklines--}

Readonly. Gets the collection of [Sparkline](../sparkline/) object.

```javascript
sparklines : SparklineCollection;
```


### type {#type--}

Indicates the sparkline type of the sparkline group.

```javascript
type : SparklineType;
```


### plotEmptyCellsType {#plotEmptyCellsType--}

Indicates how to plot empty cells.

```javascript
plotEmptyCellsType : PlotEmptyCellsType;
```


### displayHidden {#displayHidden--}

Indicates whether to show data in hidden rows and columns.

```javascript
displayHidden : boolean;
```


### showHighPoint {#showHighPoint--}

Indicates whether to highlight the highest points of data in the sparkline group.

```javascript
showHighPoint : boolean;
```


### highPointColor {#highPointColor--}

Gets and sets the color of the highest points of data in the sparkline group.

```javascript
highPointColor : CellsColor;
```


### showLowPoint {#showLowPoint--}

Indicates whether to highlight the lowest points of data in the sparkline group.

```javascript
showLowPoint : boolean;
```


### lowPointColor {#lowPointColor--}

Gets and sets the color of the lowest points of data in the sparkline group.

```javascript
lowPointColor : CellsColor;
```


### showNegativePoints {#showNegativePoints--}

Indicates whether to highlight the negative values on the sparkline group with a different color or marker.

```javascript
showNegativePoints : boolean;
```


### negativePointsColor {#negativePointsColor--}

Gets and sets the color of the negative values on the sparkline group.

```javascript
negativePointsColor : CellsColor;
```


### showFirstPoint {#showFirstPoint--}

Indicates whether to highlight the first point of data in the sparkline group.

```javascript
showFirstPoint : boolean;
```


### firstPointColor {#firstPointColor--}

Gets and sets the color of the first point of data in the sparkline group.

```javascript
firstPointColor : CellsColor;
```


### showLastPoint {#showLastPoint--}

Indicates whether to highlight the last point of data in the sparkline group.

```javascript
showLastPoint : boolean;
```


### lastPointColor {#lastPointColor--}

Gets and sets the color of the last point of data in the sparkline group.

```javascript
lastPointColor : CellsColor;
```


### showMarkers {#showMarkers--}

Indicates whether to highlight each point in each line sparkline in the sparkline group.

```javascript
showMarkers : boolean;
```


### markersColor {#markersColor--}

Gets and sets the color of points in each line sparkline in the sparkline group.

```javascript
markersColor : CellsColor;
```


### seriesColor {#seriesColor--}

Gets and sets the color of the sparklines in the sparkline group.

```javascript
seriesColor : CellsColor;
```


### plotRightToLeft {#plotRightToLeft--}

Indicates whether the plot data is right to left.

```javascript
plotRightToLeft : boolean;
```


### lineWeight {#lineWeight--}

Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points.

```javascript
lineWeight : number;
```


### horizontalAxisColor {#horizontalAxisColor--}

Gets and sets the color of the horizontal axis in the sparkline group.

```javascript
horizontalAxisColor : CellsColor;
```


### showHorizontalAxis {#showHorizontalAxis--}

Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that crosses the zero axis.

```javascript
showHorizontalAxis : boolean;
```


### horizontalAxisDateRange {#horizontalAxisDateRange--}

Represents the range that contains the date values for the sparkline data.

```javascript
horizontalAxisDateRange : string;
```


### verticalAxisMaxValueType {#verticalAxisMaxValueType--}

Represents the vertical axis maximum value type.

```javascript
verticalAxisMaxValueType : SparklineAxisMinMaxType;
```


### verticalAxisMaxValue {#verticalAxisMaxValue--}

Gets and sets the custom maximum value for the vertical axis.

```javascript
verticalAxisMaxValue : number;
```


**Remarks**

If this property is set, [VerticalAxisMaxValueType](../verticalaxismaxvaluetype/) will be <see  cref="SparklineAxisMinMaxType.Custom"/>.

### verticalAxisMinValueType {#verticalAxisMinValueType--}

Represents the vertical axis minimum value type.

```javascript
verticalAxisMinValueType : SparklineAxisMinMaxType;
```


### verticalAxisMinValue {#verticalAxisMinValue--}

Gets and sets the custom minimum value for the vertical axis.

```javascript
verticalAxisMinValue : number;
```


**Remarks**

If this property is set, [VerticalAxisMinValueType](../verticalaxisminvaluetype/) will be <see  cref="SparklineAxisMinMaxType.Custom"/>.

### getPresetStyle() {#getPresetStyle--}

<b>@deprecated.</b> Please use the 'presetStyle' property instead. Gets and sets the preset style type of the sparkline group.

```javascript
getPresetStyle() : SparklinePresetStyleType;
```


**Returns**

[SparklinePresetStyleType](../sparklinepresetstyletype/)

### setPresetStyle(SparklinePresetStyleType) {#setPresetStyle-sparklinepresetstyletype-}

<b>@deprecated.</b> Please use the 'presetStyle' property instead. Gets and sets the preset style type of the sparkline group.

```javascript
setPresetStyle(value: SparklinePresetStyleType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SparklinePresetStyleType](../sparklinepresetstyletype/) | The value to set. |

### getSparklines() {#getSparklines--}

<b>@deprecated.</b> Please use the 'sparklines' property instead. Gets the collection of [Sparkline](../sparkline/) object.

```javascript
getSparklines() : SparklineCollection;
```


**Returns**

[SparklineCollection](../sparklinecollection/)

### getType() {#getType--}

<b>@deprecated.</b> Please use the 'type' property instead. Indicates the sparkline type of the sparkline group.

```javascript
getType() : SparklineType;
```


**Returns**

[SparklineType](../sparklinetype/)

### setType(SparklineType) {#setType-sparklinetype-}

<b>@deprecated.</b> Please use the 'type' property instead. Indicates the sparkline type of the sparkline group.

```javascript
setType(value: SparklineType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SparklineType](../sparklinetype/) | The value to set. |

### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}

<b>@deprecated.</b> Please use the 'plotEmptyCellsType' property instead. Indicates how to plot empty cells.

```javascript
getPlotEmptyCellsType() : PlotEmptyCellsType;
```


**Returns**

[PlotEmptyCellsType](../plotemptycellstype/)

### setPlotEmptyCellsType(PlotEmptyCellsType) {#setPlotEmptyCellsType-plotemptycellstype-}

<b>@deprecated.</b> Please use the 'plotEmptyCellsType' property instead. Indicates how to plot empty cells.

```javascript
setPlotEmptyCellsType(value: PlotEmptyCellsType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PlotEmptyCellsType](../plotemptycellstype/) | The value to set. |

### getDisplayHidden() {#getDisplayHidden--}

<b>@deprecated.</b> Please use the 'displayHidden' property instead. Indicates whether to show data in hidden rows and columns.

```javascript
getDisplayHidden() : boolean;
```


### setDisplayHidden(boolean) {#setDisplayHidden-boolean-}

<b>@deprecated.</b> Please use the 'displayHidden' property instead. Indicates whether to show data in hidden rows and columns.

```javascript
setDisplayHidden(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowHighPoint() {#getShowHighPoint--}

<b>@deprecated.</b> Please use the 'showHighPoint' property instead. Indicates whether to highlight the highest points of data in the sparkline group.

```javascript
getShowHighPoint() : boolean;
```


### setShowHighPoint(boolean) {#setShowHighPoint-boolean-}

<b>@deprecated.</b> Please use the 'showHighPoint' property instead. Indicates whether to highlight the highest points of data in the sparkline group.

```javascript
setShowHighPoint(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHighPointColor() {#getHighPointColor--}

<b>@deprecated.</b> Please use the 'highPointColor' property instead. Gets and sets the color of the highest points of data in the sparkline group.

```javascript
getHighPointColor() : CellsColor;
```


**Returns**

[CellsColor](../cellscolor/)

### setHighPointColor(CellsColor) {#setHighPointColor-cellscolor-}

<b>@deprecated.</b> Please use the 'highPointColor' property instead. Gets and sets the color of the highest points of data in the sparkline group.

```javascript
setHighPointColor(value: CellsColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../cellscolor/) | The value to set. |

### getShowLowPoint() {#getShowLowPoint--}

<b>@deprecated.</b> Please use the 'showLowPoint' property instead. Indicates whether to highlight the lowest points of data in the sparkline group.

```javascript
getShowLowPoint() : boolean;
```


### setShowLowPoint(boolean) {#setShowLowPoint-boolean-}

<b>@deprecated.</b> Please use the 'showLowPoint' property instead. Indicates whether to highlight the lowest points of data in the sparkline group.

```javascript
setShowLowPoint(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getLowPointColor() {#getLowPointColor--}

<b>@deprecated.</b> Please use the 'lowPointColor' property instead. Gets and sets the color of the lowest points of data in the sparkline group.

```javascript
getLowPointColor() : CellsColor;
```


**Returns**

[CellsColor](../cellscolor/)

### setLowPointColor(CellsColor) {#setLowPointColor-cellscolor-}

<b>@deprecated.</b> Please use the 'lowPointColor' property instead. Gets and sets the color of the lowest points of data in the sparkline group.

```javascript
setLowPointColor(value: CellsColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../cellscolor/) | The value to set. |

### getShowNegativePoints() {#getShowNegativePoints--}

<b>@deprecated.</b> Please use the 'showNegativePoints' property instead. Indicates whether to highlight the negative values on the sparkline group with a different color or marker.

```javascript
getShowNegativePoints() : boolean;
```


### setShowNegativePoints(boolean) {#setShowNegativePoints-boolean-}

<b>@deprecated.</b> Please use the 'showNegativePoints' property instead. Indicates whether to highlight the negative values on the sparkline group with a different color or marker.

```javascript
setShowNegativePoints(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getNegativePointsColor() {#getNegativePointsColor--}

<b>@deprecated.</b> Please use the 'negativePointsColor' property instead. Gets and sets the color of the negative values on the sparkline group.

```javascript
getNegativePointsColor() : CellsColor;
```


**Returns**

[CellsColor](../cellscolor/)

### setNegativePointsColor(CellsColor) {#setNegativePointsColor-cellscolor-}

<b>@deprecated.</b> Please use the 'negativePointsColor' property instead. Gets and sets the color of the negative values on the sparkline group.

```javascript
setNegativePointsColor(value: CellsColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../cellscolor/) | The value to set. |

### getShowFirstPoint() {#getShowFirstPoint--}

<b>@deprecated.</b> Please use the 'showFirstPoint' property instead. Indicates whether to highlight the first point of data in the sparkline group.

```javascript
getShowFirstPoint() : boolean;
```


### setShowFirstPoint(boolean) {#setShowFirstPoint-boolean-}

<b>@deprecated.</b> Please use the 'showFirstPoint' property instead. Indicates whether to highlight the first point of data in the sparkline group.

```javascript
setShowFirstPoint(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFirstPointColor() {#getFirstPointColor--}

<b>@deprecated.</b> Please use the 'firstPointColor' property instead. Gets and sets the color of the first point of data in the sparkline group.

```javascript
getFirstPointColor() : CellsColor;
```


**Returns**

[CellsColor](../cellscolor/)

### setFirstPointColor(CellsColor) {#setFirstPointColor-cellscolor-}

<b>@deprecated.</b> Please use the 'firstPointColor' property instead. Gets and sets the color of the first point of data in the sparkline group.

```javascript
setFirstPointColor(value: CellsColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../cellscolor/) | The value to set. |

### getShowLastPoint() {#getShowLastPoint--}

<b>@deprecated.</b> Please use the 'showLastPoint' property instead. Indicates whether to highlight the last point of data in the sparkline group.

```javascript
getShowLastPoint() : boolean;
```


### setShowLastPoint(boolean) {#setShowLastPoint-boolean-}

<b>@deprecated.</b> Please use the 'showLastPoint' property instead. Indicates whether to highlight the last point of data in the sparkline group.

```javascript
setShowLastPoint(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getLastPointColor() {#getLastPointColor--}

<b>@deprecated.</b> Please use the 'lastPointColor' property instead. Gets and sets the color of the last point of data in the sparkline group.

```javascript
getLastPointColor() : CellsColor;
```


**Returns**

[CellsColor](../cellscolor/)

### setLastPointColor(CellsColor) {#setLastPointColor-cellscolor-}

<b>@deprecated.</b> Please use the 'lastPointColor' property instead. Gets and sets the color of the last point of data in the sparkline group.

```javascript
setLastPointColor(value: CellsColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../cellscolor/) | The value to set. |

### getShowMarkers() {#getShowMarkers--}

<b>@deprecated.</b> Please use the 'showMarkers' property instead. Indicates whether to highlight each point in each line sparkline in the sparkline group.

```javascript
getShowMarkers() : boolean;
```


### setShowMarkers(boolean) {#setShowMarkers-boolean-}

<b>@deprecated.</b> Please use the 'showMarkers' property instead. Indicates whether to highlight each point in each line sparkline in the sparkline group.

```javascript
setShowMarkers(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMarkersColor() {#getMarkersColor--}

<b>@deprecated.</b> Please use the 'markersColor' property instead. Gets and sets the color of points in each line sparkline in the sparkline group.

```javascript
getMarkersColor() : CellsColor;
```


**Returns**

[CellsColor](../cellscolor/)

### setMarkersColor(CellsColor) {#setMarkersColor-cellscolor-}

<b>@deprecated.</b> Please use the 'markersColor' property instead. Gets and sets the color of points in each line sparkline in the sparkline group.

```javascript
setMarkersColor(value: CellsColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../cellscolor/) | The value to set. |

### getSeriesColor() {#getSeriesColor--}

<b>@deprecated.</b> Please use the 'seriesColor' property instead. Gets and sets the color of the sparklines in the sparkline group.

```javascript
getSeriesColor() : CellsColor;
```


**Returns**

[CellsColor](../cellscolor/)

### setSeriesColor(CellsColor) {#setSeriesColor-cellscolor-}

<b>@deprecated.</b> Please use the 'seriesColor' property instead. Gets and sets the color of the sparklines in the sparkline group.

```javascript
setSeriesColor(value: CellsColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../cellscolor/) | The value to set. |

### getPlotRightToLeft() {#getPlotRightToLeft--}

<b>@deprecated.</b> Please use the 'plotRightToLeft' property instead. Indicates whether the plot data is right to left.

```javascript
getPlotRightToLeft() : boolean;
```


### setPlotRightToLeft(boolean) {#setPlotRightToLeft-boolean-}

<b>@deprecated.</b> Please use the 'plotRightToLeft' property instead. Indicates whether the plot data is right to left.

```javascript
setPlotRightToLeft(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getLineWeight() {#getLineWeight--}

<b>@deprecated.</b> Please use the 'lineWeight' property instead. Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points.

```javascript
getLineWeight() : number;
```


### setLineWeight(number) {#setLineWeight-number-}

<b>@deprecated.</b> Please use the 'lineWeight' property instead. Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points.

```javascript
setLineWeight(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHorizontalAxisColor() {#getHorizontalAxisColor--}

<b>@deprecated.</b> Please use the 'horizontalAxisColor' property instead. Gets and sets the color of the horizontal axis in the sparkline group.

```javascript
getHorizontalAxisColor() : CellsColor;
```


**Returns**

[CellsColor](../cellscolor/)

### setHorizontalAxisColor(CellsColor) {#setHorizontalAxisColor-cellscolor-}

<b>@deprecated.</b> Please use the 'horizontalAxisColor' property instead. Gets and sets the color of the horizontal axis in the sparkline group.

```javascript
setHorizontalAxisColor(value: CellsColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../cellscolor/) | The value to set. |

### getShowHorizontalAxis() {#getShowHorizontalAxis--}

<b>@deprecated.</b> Please use the 'showHorizontalAxis' property instead. Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that crosses the zero axis.

```javascript
getShowHorizontalAxis() : boolean;
```


### setShowHorizontalAxis(boolean) {#setShowHorizontalAxis-boolean-}

<b>@deprecated.</b> Please use the 'showHorizontalAxis' property instead. Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that crosses the zero axis.

```javascript
setShowHorizontalAxis(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHorizontalAxisDateRange() {#getHorizontalAxisDateRange--}

<b>@deprecated.</b> Please use the 'horizontalAxisDateRange' property instead. Represents the range that contains the date values for the sparkline data.

```javascript
getHorizontalAxisDateRange() : string;
```


### setHorizontalAxisDateRange(string) {#setHorizontalAxisDateRange-string-}

<b>@deprecated.</b> Please use the 'horizontalAxisDateRange' property instead. Represents the range that contains the date values for the sparkline data.

```javascript
setHorizontalAxisDateRange(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getVerticalAxisMaxValueType() {#getVerticalAxisMaxValueType--}

<b>@deprecated.</b> Please use the 'verticalAxisMaxValueType' property instead. Represents the vertical axis maximum value type.

```javascript
getVerticalAxisMaxValueType() : SparklineAxisMinMaxType;
```


**Returns**

[SparklineAxisMinMaxType](../sparklineaxisminmaxtype/)

### setVerticalAxisMaxValueType(SparklineAxisMinMaxType) {#setVerticalAxisMaxValueType-sparklineaxisminmaxtype-}

<b>@deprecated.</b> Please use the 'verticalAxisMaxValueType' property instead. Represents the vertical axis maximum value type.

```javascript
setVerticalAxisMaxValueType(value: SparklineAxisMinMaxType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SparklineAxisMinMaxType](../sparklineaxisminmaxtype/) | The value to set. |

### getVerticalAxisMaxValue() {#getVerticalAxisMaxValue--}

<b>@deprecated.</b> Please use the 'verticalAxisMaxValue' property instead. Gets and sets the custom maximum value for the vertical axis.

```javascript
getVerticalAxisMaxValue() : number;
```


**Remarks**

If this property is set, [VerticalAxisMaxValueType](../verticalaxismaxvaluetype/) will be <see  cref="SparklineAxisMinMaxType.Custom"/>.

### setVerticalAxisMaxValue(number) {#setVerticalAxisMaxValue-number-}

<b>@deprecated.</b> Please use the 'verticalAxisMaxValue' property instead. Gets and sets the custom maximum value for the vertical axis.

```javascript
setVerticalAxisMaxValue(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

If this property is set, [VerticalAxisMaxValueType](../verticalaxismaxvaluetype/) will be <see  cref="SparklineAxisMinMaxType.Custom"/>.

### getVerticalAxisMinValueType() {#getVerticalAxisMinValueType--}

<b>@deprecated.</b> Please use the 'verticalAxisMinValueType' property instead. Represents the vertical axis minimum value type.

```javascript
getVerticalAxisMinValueType() : SparklineAxisMinMaxType;
```


**Returns**

[SparklineAxisMinMaxType](../sparklineaxisminmaxtype/)

### setVerticalAxisMinValueType(SparklineAxisMinMaxType) {#setVerticalAxisMinValueType-sparklineaxisminmaxtype-}

<b>@deprecated.</b> Please use the 'verticalAxisMinValueType' property instead. Represents the vertical axis minimum value type.

```javascript
setVerticalAxisMinValueType(value: SparklineAxisMinMaxType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SparklineAxisMinMaxType](../sparklineaxisminmaxtype/) | The value to set. |

### getVerticalAxisMinValue() {#getVerticalAxisMinValue--}

<b>@deprecated.</b> Please use the 'verticalAxisMinValue' property instead. Gets and sets the custom minimum value for the vertical axis.

```javascript
getVerticalAxisMinValue() : number;
```


**Remarks**

If this property is set, [VerticalAxisMinValueType](../verticalaxisminvaluetype/) will be <see  cref="SparklineAxisMinMaxType.Custom"/>.

### setVerticalAxisMinValue(number) {#setVerticalAxisMinValue-number-}

<b>@deprecated.</b> Please use the 'verticalAxisMinValue' property instead. Gets and sets the custom minimum value for the vertical axis.

```javascript
setVerticalAxisMinValue(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

If this property is set, [VerticalAxisMinValueType](../verticalaxisminvaluetype/) will be <see  cref="SparklineAxisMinMaxType.Custom"/>.

### resetRanges(string, boolean, CellArea) {#resetRanges-string-boolean-cellarea-}

Resets the data range and location range of the sparkline group. This method will clear original sparkline items in the group and creates new sparkline items for the new ranges.

```javascript
resetRanges(dataRange: string, isVertical: boolean, locationRange: CellArea) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dataRange | string | Specifies the new data range of the sparkline group. |
| isVertical | boolean | Specifies whether to plot the sparklines from the new data range by row or by column. |
| locationRange | [CellArea](../cellarea/) | Specifies where the sparklines to be placed. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



