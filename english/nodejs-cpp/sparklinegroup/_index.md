---
title: SparklineGroup
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Sparklinenodejscppsparkline is organized into sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type display settings and axis settings for the sparklines.
type: docs
url: /nodejs-cpp/sparklinegroup/
---

## SparklineGroup class

[Sparkline](/nodejs-cpp/sparkline/) is organized into sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type, display settings and axis settings for the sparklines.

```javascript
class SparklineGroup;
```


## Methods

| Method | Description |
| --- | --- |
| [getPresetStyle()](#getPresetStyle--)| Gets and sets the preset style type of the sparkline group. |
| [setPresetStyle(SparklinePresetStyleType)](#setPresetStyle-sparklinepresetstyletype-)| Gets and sets the preset style type of the sparkline group. |
| [getSparklines()](#getSparklines--)| Gets the collection of [Sparkline](/nodejs-cpp/sparkline/) object. |
| [getType()](#getType--)| Indicates the sparkline type of the sparkline group. |
| [setType(SparklineType)](#setType-sparklinetype-)| Indicates the sparkline type of the sparkline group. |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--)| Indicates how to plot empty cells. |
| [setPlotEmptyCellsType(PlotEmptyCellsType)](#setPlotEmptyCellsType-plotemptycellstype-)| Indicates how to plot empty cells. |
| [getDisplayHidden()](#getDisplayHidden--)| Indicates whether to show data in hidden rows and columns. |
| [setDisplayHidden(boolean)](#setDisplayHidden-boolean-)| Indicates whether to show data in hidden rows and columns. |
| [getShowHighPoint()](#getShowHighPoint--)| Indicates whether to highlight the highest points of data in the sparkline group. |
| [setShowHighPoint(boolean)](#setShowHighPoint-boolean-)| Indicates whether to highlight the highest points of data in the sparkline group. |
| [getHighPointColor()](#getHighPointColor--)| Gets and sets the color of the highest points of data in the sparkline group. |
| [setHighPointColor(CellsColor)](#setHighPointColor-cellscolor-)| Gets and sets the color of the highest points of data in the sparkline group. |
| [getShowLowPoint()](#getShowLowPoint--)| Indicates whether to highlight the lowest points of data in the sparkline group. |
| [setShowLowPoint(boolean)](#setShowLowPoint-boolean-)| Indicates whether to highlight the lowest points of data in the sparkline group. |
| [getLowPointColor()](#getLowPointColor--)| Gets and sets the color of the lowest points of data in the sparkline group. |
| [setLowPointColor(CellsColor)](#setLowPointColor-cellscolor-)| Gets and sets the color of the lowest points of data in the sparkline group. |
| [getShowNegativePoints()](#getShowNegativePoints--)| Indicates whether to highlight the negative values on the sparkline group with a different color or marker. |
| [setShowNegativePoints(boolean)](#setShowNegativePoints-boolean-)| Indicates whether to highlight the negative values on the sparkline group with a different color or marker. |
| [getNegativePointsColor()](#getNegativePointsColor--)| Gets and sets the color of the negative values on the sparkline group. |
| [setNegativePointsColor(CellsColor)](#setNegativePointsColor-cellscolor-)| Gets and sets the color of the negative values on the sparkline group. |
| [getShowFirstPoint()](#getShowFirstPoint--)| Indicates whether to highlight the first point of data in the sparkline group. |
| [setShowFirstPoint(boolean)](#setShowFirstPoint-boolean-)| Indicates whether to highlight the first point of data in the sparkline group. |
| [getFirstPointColor()](#getFirstPointColor--)| Gets and sets the color of the first point of data in the sparkline group. |
| [setFirstPointColor(CellsColor)](#setFirstPointColor-cellscolor-)| Gets and sets the color of the first point of data in the sparkline group. |
| [getShowLastPoint()](#getShowLastPoint--)| Indicates whether to highlight the last point of data in the sparkline group. |
| [setShowLastPoint(boolean)](#setShowLastPoint-boolean-)| Indicates whether to highlight the last point of data in the sparkline group. |
| [getLastPointColor()](#getLastPointColor--)| Gets and sets the color of the last point of data in the sparkline group. |
| [setLastPointColor(CellsColor)](#setLastPointColor-cellscolor-)| Gets and sets the color of the last point of data in the sparkline group. |
| [getShowMarkers()](#getShowMarkers--)| Indicates whether to highlight each point in each line sparkline in the sparkline group. |
| [setShowMarkers(boolean)](#setShowMarkers-boolean-)| Indicates whether to highlight each point in each line sparkline in the sparkline group. |
| [getMarkersColor()](#getMarkersColor--)| Gets and sets the color of points in each line sparkline in the sparkline group. |
| [setMarkersColor(CellsColor)](#setMarkersColor-cellscolor-)| Gets and sets the color of points in each line sparkline in the sparkline group. |
| [getSeriesColor()](#getSeriesColor--)| Gets and sets the color of the sparklines in the sparkline group. |
| [setSeriesColor(CellsColor)](#setSeriesColor-cellscolor-)| Gets and sets the color of the sparklines in the sparkline group. |
| [getPlotRightToLeft()](#getPlotRightToLeft--)| Indicates whether the plot data is right to left. |
| [setPlotRightToLeft(boolean)](#setPlotRightToLeft-boolean-)| Indicates whether the plot data is right to left. |
| [getLineWeight()](#getLineWeight--)| Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points. |
| [setLineWeight(number)](#setLineWeight-number-)| Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points. |
| [getHorizontalAxisColor()](#getHorizontalAxisColor--)| Gets and sets the color of the horizontal axis in the sparkline group. |
| [setHorizontalAxisColor(CellsColor)](#setHorizontalAxisColor-cellscolor-)| Gets and sets the color of the horizontal axis in the sparkline group. |
| [getShowHorizontalAxis()](#getShowHorizontalAxis--)| Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that crosses the zero axis. |
| [setShowHorizontalAxis(boolean)](#setShowHorizontalAxis-boolean-)| Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that crosses the zero axis. |
| [getHorizontalAxisDateRange()](#getHorizontalAxisDateRange--)| Represents the range that contains the date values for the sparkline data. |
| [setHorizontalAxisDateRange(string)](#setHorizontalAxisDateRange-string-)| Represents the range that contains the date values for the sparkline data. |
| [getVerticalAxisMaxValueType()](#getVerticalAxisMaxValueType--)| Represents the vertical axis maximum value type. |
| [setVerticalAxisMaxValueType(SparklineAxisMinMaxType)](#setVerticalAxisMaxValueType-sparklineaxisminmaxtype-)| Represents the vertical axis maximum value type. |
| [getVerticalAxisMaxValue()](#getVerticalAxisMaxValue--)| Gets and sets the custom maximum value for the vertical axis. |
| [setVerticalAxisMaxValue(number)](#setVerticalAxisMaxValue-number-)| Gets and sets the custom maximum value for the vertical axis. |
| [getVerticalAxisMinValueType()](#getVerticalAxisMinValueType--)| Represents the vertical axis minimum value type. |
| [setVerticalAxisMinValueType(SparklineAxisMinMaxType)](#setVerticalAxisMinValueType-sparklineaxisminmaxtype-)| Represents the vertical axis minimum value type. |
| [getVerticalAxisMinValue()](#getVerticalAxisMinValue--)| Gets and sets the custom minimum value for the vertical axis. |
| [setVerticalAxisMinValue(number)](#setVerticalAxisMinValue-number-)| Gets and sets the custom minimum value for the vertical axis. |
| [resetRanges(string, boolean, CellArea)](#resetRanges-string-boolean-cellarea-)| Resets the data range and location range of the sparkline group. This method will clear original sparkline items in the group and creates new sparkline items for the new ranges. |


### getPresetStyle() {#getPresetStyle--}

Gets and sets the preset style type of the sparkline group.

```javascript
getPresetStyle() : SparklinePresetStyleType;
```


**Returns**

[SparklinePresetStyleType](/nodejs-cpp/sparklinepresetstyletype/)

### setPresetStyle(SparklinePresetStyleType) {#setPresetStyle-sparklinepresetstyletype-}

Gets and sets the preset style type of the sparkline group.

```javascript
setPresetStyle(value: SparklinePresetStyleType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SparklinePresetStyleType](/nodejs-cpp/sparklinepresetstyletype/) | The value to set. |

### getSparklines() {#getSparklines--}

Gets the collection of [Sparkline](/nodejs-cpp/sparkline/) object.

```javascript
getSparklines() : SparklineCollection;
```


**Returns**

[SparklineCollection](/nodejs-cpp/sparklinecollection/)

### getType() {#getType--}

Indicates the sparkline type of the sparkline group.

```javascript
getType() : SparklineType;
```


**Returns**

[SparklineType](/nodejs-cpp/sparklinetype/)

### setType(SparklineType) {#setType-sparklinetype-}

Indicates the sparkline type of the sparkline group.

```javascript
setType(value: SparklineType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SparklineType](/nodejs-cpp/sparklinetype/) | The value to set. |

### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}

Indicates how to plot empty cells.

```javascript
getPlotEmptyCellsType() : PlotEmptyCellsType;
```


**Returns**

[PlotEmptyCellsType](/nodejs-cpp/plotemptycellstype/)

### setPlotEmptyCellsType(PlotEmptyCellsType) {#setPlotEmptyCellsType-plotemptycellstype-}

Indicates how to plot empty cells.

```javascript
setPlotEmptyCellsType(value: PlotEmptyCellsType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PlotEmptyCellsType](/nodejs-cpp/plotemptycellstype/) | The value to set. |

### getDisplayHidden() {#getDisplayHidden--}

Indicates whether to show data in hidden rows and columns.

```javascript
getDisplayHidden() : boolean;
```


### setDisplayHidden(boolean) {#setDisplayHidden-boolean-}

Indicates whether to show data in hidden rows and columns.

```javascript
setDisplayHidden(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowHighPoint() {#getShowHighPoint--}

Indicates whether to highlight the highest points of data in the sparkline group.

```javascript
getShowHighPoint() : boolean;
```


### setShowHighPoint(boolean) {#setShowHighPoint-boolean-}

Indicates whether to highlight the highest points of data in the sparkline group.

```javascript
setShowHighPoint(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHighPointColor() {#getHighPointColor--}

Gets and sets the color of the highest points of data in the sparkline group.

```javascript
getHighPointColor() : CellsColor;
```


**Returns**

[CellsColor](/nodejs-cpp/cellscolor/)

### setHighPointColor(CellsColor) {#setHighPointColor-cellscolor-}

Gets and sets the color of the highest points of data in the sparkline group.

```javascript
setHighPointColor(value: CellsColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](/nodejs-cpp/cellscolor/) | The value to set. |

### getShowLowPoint() {#getShowLowPoint--}

Indicates whether to highlight the lowest points of data in the sparkline group.

```javascript
getShowLowPoint() : boolean;
```


### setShowLowPoint(boolean) {#setShowLowPoint-boolean-}

Indicates whether to highlight the lowest points of data in the sparkline group.

```javascript
setShowLowPoint(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getLowPointColor() {#getLowPointColor--}

Gets and sets the color of the lowest points of data in the sparkline group.

```javascript
getLowPointColor() : CellsColor;
```


**Returns**

[CellsColor](/nodejs-cpp/cellscolor/)

### setLowPointColor(CellsColor) {#setLowPointColor-cellscolor-}

Gets and sets the color of the lowest points of data in the sparkline group.

```javascript
setLowPointColor(value: CellsColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](/nodejs-cpp/cellscolor/) | The value to set. |

### getShowNegativePoints() {#getShowNegativePoints--}

Indicates whether to highlight the negative values on the sparkline group with a different color or marker.

```javascript
getShowNegativePoints() : boolean;
```


### setShowNegativePoints(boolean) {#setShowNegativePoints-boolean-}

Indicates whether to highlight the negative values on the sparkline group with a different color or marker.

```javascript
setShowNegativePoints(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getNegativePointsColor() {#getNegativePointsColor--}

Gets and sets the color of the negative values on the sparkline group.

```javascript
getNegativePointsColor() : CellsColor;
```


**Returns**

[CellsColor](/nodejs-cpp/cellscolor/)

### setNegativePointsColor(CellsColor) {#setNegativePointsColor-cellscolor-}

Gets and sets the color of the negative values on the sparkline group.

```javascript
setNegativePointsColor(value: CellsColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](/nodejs-cpp/cellscolor/) | The value to set. |

### getShowFirstPoint() {#getShowFirstPoint--}

Indicates whether to highlight the first point of data in the sparkline group.

```javascript
getShowFirstPoint() : boolean;
```


### setShowFirstPoint(boolean) {#setShowFirstPoint-boolean-}

Indicates whether to highlight the first point of data in the sparkline group.

```javascript
setShowFirstPoint(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFirstPointColor() {#getFirstPointColor--}

Gets and sets the color of the first point of data in the sparkline group.

```javascript
getFirstPointColor() : CellsColor;
```


**Returns**

[CellsColor](/nodejs-cpp/cellscolor/)

### setFirstPointColor(CellsColor) {#setFirstPointColor-cellscolor-}

Gets and sets the color of the first point of data in the sparkline group.

```javascript
setFirstPointColor(value: CellsColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](/nodejs-cpp/cellscolor/) | The value to set. |

### getShowLastPoint() {#getShowLastPoint--}

Indicates whether to highlight the last point of data in the sparkline group.

```javascript
getShowLastPoint() : boolean;
```


### setShowLastPoint(boolean) {#setShowLastPoint-boolean-}

Indicates whether to highlight the last point of data in the sparkline group.

```javascript
setShowLastPoint(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getLastPointColor() {#getLastPointColor--}

Gets and sets the color of the last point of data in the sparkline group.

```javascript
getLastPointColor() : CellsColor;
```


**Returns**

[CellsColor](/nodejs-cpp/cellscolor/)

### setLastPointColor(CellsColor) {#setLastPointColor-cellscolor-}

Gets and sets the color of the last point of data in the sparkline group.

```javascript
setLastPointColor(value: CellsColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](/nodejs-cpp/cellscolor/) | The value to set. |

### getShowMarkers() {#getShowMarkers--}

Indicates whether to highlight each point in each line sparkline in the sparkline group.

```javascript
getShowMarkers() : boolean;
```


### setShowMarkers(boolean) {#setShowMarkers-boolean-}

Indicates whether to highlight each point in each line sparkline in the sparkline group.

```javascript
setShowMarkers(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMarkersColor() {#getMarkersColor--}

Gets and sets the color of points in each line sparkline in the sparkline group.

```javascript
getMarkersColor() : CellsColor;
```


**Returns**

[CellsColor](/nodejs-cpp/cellscolor/)

### setMarkersColor(CellsColor) {#setMarkersColor-cellscolor-}

Gets and sets the color of points in each line sparkline in the sparkline group.

```javascript
setMarkersColor(value: CellsColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](/nodejs-cpp/cellscolor/) | The value to set. |

### getSeriesColor() {#getSeriesColor--}

Gets and sets the color of the sparklines in the sparkline group.

```javascript
getSeriesColor() : CellsColor;
```


**Returns**

[CellsColor](/nodejs-cpp/cellscolor/)

### setSeriesColor(CellsColor) {#setSeriesColor-cellscolor-}

Gets and sets the color of the sparklines in the sparkline group.

```javascript
setSeriesColor(value: CellsColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](/nodejs-cpp/cellscolor/) | The value to set. |

### getPlotRightToLeft() {#getPlotRightToLeft--}

Indicates whether the plot data is right to left.

```javascript
getPlotRightToLeft() : boolean;
```


### setPlotRightToLeft(boolean) {#setPlotRightToLeft-boolean-}

Indicates whether the plot data is right to left.

```javascript
setPlotRightToLeft(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getLineWeight() {#getLineWeight--}

Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points.

```javascript
getLineWeight() : number;
```


### setLineWeight(number) {#setLineWeight-number-}

Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points.

```javascript
setLineWeight(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHorizontalAxisColor() {#getHorizontalAxisColor--}

Gets and sets the color of the horizontal axis in the sparkline group.

```javascript
getHorizontalAxisColor() : CellsColor;
```


**Returns**

[CellsColor](/nodejs-cpp/cellscolor/)

### setHorizontalAxisColor(CellsColor) {#setHorizontalAxisColor-cellscolor-}

Gets and sets the color of the horizontal axis in the sparkline group.

```javascript
setHorizontalAxisColor(value: CellsColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](/nodejs-cpp/cellscolor/) | The value to set. |

### getShowHorizontalAxis() {#getShowHorizontalAxis--}

Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that crosses the zero axis.

```javascript
getShowHorizontalAxis() : boolean;
```


### setShowHorizontalAxis(boolean) {#setShowHorizontalAxis-boolean-}

Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that crosses the zero axis.

```javascript
setShowHorizontalAxis(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHorizontalAxisDateRange() {#getHorizontalAxisDateRange--}

Represents the range that contains the date values for the sparkline data.

```javascript
getHorizontalAxisDateRange() : string;
```


### setHorizontalAxisDateRange(string) {#setHorizontalAxisDateRange-string-}

Represents the range that contains the date values for the sparkline data.

```javascript
setHorizontalAxisDateRange(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getVerticalAxisMaxValueType() {#getVerticalAxisMaxValueType--}

Represents the vertical axis maximum value type.

```javascript
getVerticalAxisMaxValueType() : SparklineAxisMinMaxType;
```


**Returns**

[SparklineAxisMinMaxType](/nodejs-cpp/sparklineaxisminmaxtype/)

### setVerticalAxisMaxValueType(SparklineAxisMinMaxType) {#setVerticalAxisMaxValueType-sparklineaxisminmaxtype-}

Represents the vertical axis maximum value type.

```javascript
setVerticalAxisMaxValueType(value: SparklineAxisMinMaxType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SparklineAxisMinMaxType](/nodejs-cpp/sparklineaxisminmaxtype/) | The value to set. |

### getVerticalAxisMaxValue() {#getVerticalAxisMaxValue--}

Gets and sets the custom maximum value for the vertical axis.

```javascript
getVerticalAxisMaxValue() : number;
```


### setVerticalAxisMaxValue(number) {#setVerticalAxisMaxValue-number-}

Gets and sets the custom maximum value for the vertical axis.

```javascript
setVerticalAxisMaxValue(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getVerticalAxisMinValueType() {#getVerticalAxisMinValueType--}

Represents the vertical axis minimum value type.

```javascript
getVerticalAxisMinValueType() : SparklineAxisMinMaxType;
```


**Returns**

[SparklineAxisMinMaxType](/nodejs-cpp/sparklineaxisminmaxtype/)

### setVerticalAxisMinValueType(SparklineAxisMinMaxType) {#setVerticalAxisMinValueType-sparklineaxisminmaxtype-}

Represents the vertical axis minimum value type.

```javascript
setVerticalAxisMinValueType(value: SparklineAxisMinMaxType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SparklineAxisMinMaxType](/nodejs-cpp/sparklineaxisminmaxtype/) | The value to set. |

### getVerticalAxisMinValue() {#getVerticalAxisMinValue--}

Gets and sets the custom minimum value for the vertical axis.

```javascript
getVerticalAxisMinValue() : number;
```


### setVerticalAxisMinValue(number) {#setVerticalAxisMinValue-number-}

Gets and sets the custom minimum value for the vertical axis.

```javascript
setVerticalAxisMinValue(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

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
| locationRange | [CellArea](/nodejs-cpp/cellarea/) | Specifies where the sparklines to be placed. |


