---
title: Axis
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents an axis of chart.
type: docs
url: /nodejs-cpp/axis/
---

## Axis class

Encapsulates the object that represents an axis of chart.

```javascript
class Axis;
```


## Methods

| Method | Description |
| --- | --- |
| [getArea()](#getArea--)| Gets the [Area](../area/). |
| [isAutomaticMinValue()](#isAutomaticMinValue--)| Indicates whether the min value is automatically assigned. |
| [setIsAutomaticMinValue(boolean)](#setIsAutomaticMinValue-boolean-)| Indicates whether the min value is automatically assigned. |
| [getMinValue()](#getMinValue--)| Represents the minimum value on the value axis. |
| [setMinValue(object)](#setMinValue-object-)| Represents the minimum value on the value axis. |
| [isAutomaticMaxValue()](#isAutomaticMaxValue--)| Indicates whether the max value is automatically assigned. |
| [setIsAutomaticMaxValue(boolean)](#setIsAutomaticMaxValue-boolean-)| Indicates whether the max value is automatically assigned. |
| [getMaxValue()](#getMaxValue--)| Represents the maximum value on the value axis. |
| [setMaxValue(object)](#setMaxValue-object-)| Represents the maximum value on the value axis. |
| [isAutomaticMajorUnit()](#isAutomaticMajorUnit--)| Indicates whether the major unit of the axis is automatically assigned. |
| [setIsAutomaticMajorUnit(boolean)](#setIsAutomaticMajorUnit-boolean-)| Indicates whether the major unit of the axis is automatically assigned. |
| [getMajorUnit()](#getMajorUnit--)| Represents the major units for the axis. |
| [setMajorUnit(number)](#setMajorUnit-number-)| Represents the major units for the axis. |
| [isAutomaticMinorUnit()](#isAutomaticMinorUnit--)| Indicates whether the minor unit of the axis is automatically assigned. |
| [setIsAutomaticMinorUnit(boolean)](#setIsAutomaticMinorUnit-boolean-)| Indicates whether the minor unit of the axis is automatically assigned. |
| [getMinorUnit()](#getMinorUnit--)| Represents the minor units for the axis. |
| [setMinorUnit(number)](#setMinorUnit-number-)| Represents the minor units for the axis. |
| [getAxisLine()](#getAxisLine--)| Gets the appearance of an Axis. |
| [getMajorTickMark()](#getMajorTickMark--)| Represents the type of major tick mark for the specified axis. |
| [setMajorTickMark(TickMarkType)](#setMajorTickMark-tickmarktype-)| Represents the type of major tick mark for the specified axis. |
| [getMinorTickMark()](#getMinorTickMark--)| Represents the type of minor tick mark for the specified axis. |
| [setMinorTickMark(TickMarkType)](#setMinorTickMark-tickmarktype-)| Represents the type of minor tick mark for the specified axis. |
| [getTickLabelPosition()](#getTickLabelPosition--)| Represents the position of tick-mark labels on the specified axis. |
| [setTickLabelPosition(TickLabelPositionType)](#setTickLabelPosition-ticklabelpositiontype-)| Represents the position of tick-mark labels on the specified axis. |
| [getCrossAt()](#getCrossAt--)| Represents the point on the value axis where the category axis crosses it. |
| [setCrossAt(number)](#setCrossAt-number-)| Represents the point on the value axis where the category axis crosses it. |
| [getCrossType()](#getCrossType--)| Represents the [CrossType](../crosstype/) on the specified axis where the other axis crosses. |
| [setCrossType(CrossType)](#setCrossType-crosstype-)| Represents the [CrossType](../crosstype/) on the specified axis where the other axis crosses. |
| [getLogBase()](#getLogBase--)| Represents the logarithmic base. Default value is 10.Only applies for Excel2007. |
| [setLogBase(number)](#setLogBase-number-)| Represents the logarithmic base. Default value is 10.Only applies for Excel2007. |
| [isLogarithmic()](#isLogarithmic--)| Represents if the value axis scale type is logarithmic or not. |
| [setIsLogarithmic(boolean)](#setIsLogarithmic-boolean-)| Represents if the value axis scale type is logarithmic or not. |
| [isPlotOrderReversed()](#isPlotOrderReversed--)| Represents if Microsoft Excel plots data points from last to first. |
| [setIsPlotOrderReversed(boolean)](#setIsPlotOrderReversed-boolean-)| Represents if Microsoft Excel plots data points from last to first. |
| [getAxisBetweenCategories()](#getAxisBetweenCategories--)| Represents if the value axis crosses the category axis between categories. |
| [setAxisBetweenCategories(boolean)](#setAxisBetweenCategories-boolean-)| Represents if the value axis crosses the category axis between categories. |
| [getTickLabels()](#getTickLabels--)| Returns a [TickLabels](../ticklabels/) object that represents the tick-mark labels for the specified axis. |
| [getTickLabelSpacing()](#getTickLabelSpacing--)| Represents the number of categories or series between tick-mark labels. Applies only to category and series axes. |
| [setTickLabelSpacing(number)](#setTickLabelSpacing-number-)| Represents the number of categories or series between tick-mark labels. Applies only to category and series axes. |
| [isAutoTickLabelSpacing()](#isAutoTickLabelSpacing--)| Indicates whether the spacing of tick label is automatic |
| [setIsAutoTickLabelSpacing(boolean)](#setIsAutoTickLabelSpacing-boolean-)| Indicates whether the spacing of tick label is automatic |
| [getTickMarkSpacing()](#getTickMarkSpacing--)| Returns or sets the number of categories or series between tick marks. Applies only to category and series axes. |
| [setTickMarkSpacing(number)](#setTickMarkSpacing-number-)| Returns or sets the number of categories or series between tick marks. Applies only to category and series axes. |
| [getDisplayUnit()](#getDisplayUnit--)| Represents the unit label for the specified axis. |
| [setDisplayUnit(DisplayUnitType)](#setDisplayUnit-displayunittype-)| Represents the unit label for the specified axis. |
| [getCustomUnit()](#getCustomUnit--)| Specifies a custom value for the display unit. |
| [setCustomUnit(number)](#setCustomUnit-number-)| Specifies a custom value for the display unit. |
| [getDisplayUnitLabel()](#getDisplayUnitLabel--)| Represents a unit label on an axis in the specified chart. Unit labels are useful for charting large values— for example, in the millions or billions. |
| [isDisplayUnitLabelShown()](#isDisplayUnitLabelShown--)| Represents if the display unit label is shown on the specified axis. |
| [setIsDisplayUnitLabelShown(boolean)](#setIsDisplayUnitLabelShown-boolean-)| Represents if the display unit label is shown on the specified axis. |
| [getTitle()](#getTitle--)| Gets the axis' title. |
| [getCategoryType()](#getCategoryType--)| Represents the category axis type. |
| [setCategoryType(CategoryType)](#setCategoryType-categorytype-)| Represents the category axis type. |
| [getBaseUnitScale()](#getBaseUnitScale--)| Represents the base unit scale for the category axis. |
| [setBaseUnitScale(TimeUnit)](#setBaseUnitScale-timeunit-)| Represents the base unit scale for the category axis. |
| [getMajorUnitScale()](#getMajorUnitScale--)| Represents the major unit scale for the category axis. |
| [setMajorUnitScale(TimeUnit)](#setMajorUnitScale-timeunit-)| Represents the major unit scale for the category axis. |
| [getMinorUnitScale()](#getMinorUnitScale--)| Represents the major unit scale for the category axis. |
| [setMinorUnitScale(TimeUnit)](#setMinorUnitScale-timeunit-)| Represents the major unit scale for the category axis. |
| [isVisible()](#isVisible--)| Represents if the axis is visible. |
| [setIsVisible(boolean)](#setIsVisible-boolean-)| Represents if the axis is visible. |
| [getMajorGridLines()](#getMajorGridLines--)| Represents major gridlines on a chart axis. |
| [getMinorGridLines()](#getMinorGridLines--)| Represents minor gridlines on a chart axis. |
| [getHasMultiLevelLabels()](#getHasMultiLevelLabels--)| Indicates whether the labels shall be shown as multi level. |
| [setHasMultiLevelLabels(boolean)](#setHasMultiLevelLabels-boolean-)| Indicates whether the labels shall be shown as multi level. |
| [getBins()](#getBins--)| Represents bins on a chart(Histogram/Pareto) axis |
| [getAxisTexts()](#getAxisTexts--)| Gets the labels of the axis after call Chart.Calculate() method. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getArea() {#getArea--}

Gets the [Area](../area/).

```javascript
getArea() : Area;
```


**Returns**

[Area](../area/)

### isAutomaticMinValue() {#isAutomaticMinValue--}

Indicates whether the min value is automatically assigned.

```javascript
isAutomaticMinValue() : boolean;
```


### setIsAutomaticMinValue(boolean) {#setIsAutomaticMinValue-boolean-}

Indicates whether the min value is automatically assigned.

```javascript
setIsAutomaticMinValue(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMinValue() {#getMinValue--}

Represents the minimum value on the value axis.

```javascript
getMinValue() : object;
```


**Remarks**

The minValue type only can be double or DateTime

### setMinValue(object) {#setMinValue-object-}

Represents the minimum value on the value axis.

```javascript
setMinValue(value: object) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | object | The value to set. |

**Remarks**

The minValue type only can be double or DateTime

### isAutomaticMaxValue() {#isAutomaticMaxValue--}

Indicates whether the max value is automatically assigned.

```javascript
isAutomaticMaxValue() : boolean;
```


### setIsAutomaticMaxValue(boolean) {#setIsAutomaticMaxValue-boolean-}

Indicates whether the max value is automatically assigned.

```javascript
setIsAutomaticMaxValue(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMaxValue() {#getMaxValue--}

Represents the maximum value on the value axis.

```javascript
getMaxValue() : object;
```


**Remarks**

The maxValue type only can be double or DateTime

### setMaxValue(object) {#setMaxValue-object-}

Represents the maximum value on the value axis.

```javascript
setMaxValue(value: object) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | object | The value to set. |

**Remarks**

The maxValue type only can be double or DateTime

### isAutomaticMajorUnit() {#isAutomaticMajorUnit--}

Indicates whether the major unit of the axis is automatically assigned.

```javascript
isAutomaticMajorUnit() : boolean;
```


### setIsAutomaticMajorUnit(boolean) {#setIsAutomaticMajorUnit-boolean-}

Indicates whether the major unit of the axis is automatically assigned.

```javascript
setIsAutomaticMajorUnit(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMajorUnit() {#getMajorUnit--}

Represents the major units for the axis.

```javascript
getMajorUnit() : number;
```


**Remarks**

The major units must be greater than zero.

### setMajorUnit(number) {#setMajorUnit-number-}

Represents the major units for the axis.

```javascript
setMajorUnit(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The major units must be greater than zero.

### isAutomaticMinorUnit() {#isAutomaticMinorUnit--}

Indicates whether the minor unit of the axis is automatically assigned.

```javascript
isAutomaticMinorUnit() : boolean;
```


### setIsAutomaticMinorUnit(boolean) {#setIsAutomaticMinorUnit-boolean-}

Indicates whether the minor unit of the axis is automatically assigned.

```javascript
setIsAutomaticMinorUnit(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMinorUnit() {#getMinorUnit--}

Represents the minor units for the axis.

```javascript
getMinorUnit() : number;
```


**Remarks**

The minor units must be greater than zero.

### setMinorUnit(number) {#setMinorUnit-number-}

Represents the minor units for the axis.

```javascript
setMinorUnit(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The minor units must be greater than zero.

### getAxisLine() {#getAxisLine--}

Gets the appearance of an Axis.

```javascript
getAxisLine() : Line;
```


**Returns**

[Line](../line/)

### getMajorTickMark() {#getMajorTickMark--}

Represents the type of major tick mark for the specified axis.

```javascript
getMajorTickMark() : TickMarkType;
```


**Returns**

[TickMarkType](../tickmarktype/)

### setMajorTickMark(TickMarkType) {#setMajorTickMark-tickmarktype-}

Represents the type of major tick mark for the specified axis.

```javascript
setMajorTickMark(value: TickMarkType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TickMarkType](../tickmarktype/) | The value to set. |

### getMinorTickMark() {#getMinorTickMark--}

Represents the type of minor tick mark for the specified axis.

```javascript
getMinorTickMark() : TickMarkType;
```


**Returns**

[TickMarkType](../tickmarktype/)

### setMinorTickMark(TickMarkType) {#setMinorTickMark-tickmarktype-}

Represents the type of minor tick mark for the specified axis.

```javascript
setMinorTickMark(value: TickMarkType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TickMarkType](../tickmarktype/) | The value to set. |

### getTickLabelPosition() {#getTickLabelPosition--}

Represents the position of tick-mark labels on the specified axis.

```javascript
getTickLabelPosition() : TickLabelPositionType;
```


**Returns**

[TickLabelPositionType](../ticklabelpositiontype/)

### setTickLabelPosition(TickLabelPositionType) {#setTickLabelPosition-ticklabelpositiontype-}

Represents the position of tick-mark labels on the specified axis.

```javascript
setTickLabelPosition(value: TickLabelPositionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TickLabelPositionType](../ticklabelpositiontype/) | The value to set. |

### getCrossAt() {#getCrossAt--}

Represents the point on the value axis where the category axis crosses it.

```javascript
getCrossAt() : number;
```


**Remarks**

The number should be a integer when it applies to category axis. And the value must be between 1 and 31999.

### setCrossAt(number) {#setCrossAt-number-}

Represents the point on the value axis where the category axis crosses it.

```javascript
setCrossAt(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The number should be a integer when it applies to category axis. And the value must be between 1 and 31999.

### getCrossType() {#getCrossType--}

Represents the [CrossType](../crosstype/) on the specified axis where the other axis crosses.

```javascript
getCrossType() : CrossType;
```


**Returns**

[CrossType](../crosstype/)

### setCrossType(CrossType) {#setCrossType-crosstype-}

Represents the [CrossType](../crosstype/) on the specified axis where the other axis crosses.

```javascript
setCrossType(value: CrossType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CrossType](../crosstype/) | The value to set. |

### getLogBase() {#getLogBase--}

Represents the logarithmic base. Default value is 10.Only applies for Excel2007.

```javascript
getLogBase() : number;
```


### setLogBase(number) {#setLogBase-number-}

Represents the logarithmic base. Default value is 10.Only applies for Excel2007.

```javascript
setLogBase(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isLogarithmic() {#isLogarithmic--}

Represents if the value axis scale type is logarithmic or not.

```javascript
isLogarithmic() : boolean;
```


### setIsLogarithmic(boolean) {#setIsLogarithmic-boolean-}

Represents if the value axis scale type is logarithmic or not.

```javascript
setIsLogarithmic(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isPlotOrderReversed() {#isPlotOrderReversed--}

Represents if Microsoft Excel plots data points from last to first.

```javascript
isPlotOrderReversed() : boolean;
```


### setIsPlotOrderReversed(boolean) {#setIsPlotOrderReversed-boolean-}

Represents if Microsoft Excel plots data points from last to first.

```javascript
setIsPlotOrderReversed(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAxisBetweenCategories() {#getAxisBetweenCategories--}

Represents if the value axis crosses the category axis between categories.

```javascript
getAxisBetweenCategories() : boolean;
```


**Remarks**

This property applies only to category axes, and it doesn't apply to 3-D charts.

### setAxisBetweenCategories(boolean) {#setAxisBetweenCategories-boolean-}

Represents if the value axis crosses the category axis between categories.

```javascript
setAxisBetweenCategories(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

This property applies only to category axes, and it doesn't apply to 3-D charts.

### getTickLabels() {#getTickLabels--}

Returns a [TickLabels](../ticklabels/) object that represents the tick-mark labels for the specified axis.

```javascript
getTickLabels() : TickLabels;
```


**Returns**

[TickLabels](../ticklabels/)

### getTickLabelSpacing() {#getTickLabelSpacing--}

Represents the number of categories or series between tick-mark labels. Applies only to category and series axes.

```javascript
getTickLabelSpacing() : number;
```


**Remarks**

The number must be between 1 and 31999.

### setTickLabelSpacing(number) {#setTickLabelSpacing-number-}

Represents the number of categories or series between tick-mark labels. Applies only to category and series axes.

```javascript
setTickLabelSpacing(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The number must be between 1 and 31999.

### isAutoTickLabelSpacing() {#isAutoTickLabelSpacing--}

Indicates whether the spacing of tick label is automatic

```javascript
isAutoTickLabelSpacing() : boolean;
```


### setIsAutoTickLabelSpacing(boolean) {#setIsAutoTickLabelSpacing-boolean-}

Indicates whether the spacing of tick label is automatic

```javascript
setIsAutoTickLabelSpacing(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getTickMarkSpacing() {#getTickMarkSpacing--}

Returns or sets the number of categories or series between tick marks. Applies only to category and series axes.

```javascript
getTickMarkSpacing() : number;
```


**Remarks**

The number must be between 1 and 31999.

### setTickMarkSpacing(number) {#setTickMarkSpacing-number-}

Returns or sets the number of categories or series between tick marks. Applies only to category and series axes.

```javascript
setTickMarkSpacing(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The number must be between 1 and 31999.

### getDisplayUnit() {#getDisplayUnit--}

Represents the unit label for the specified axis.

```javascript
getDisplayUnit() : DisplayUnitType;
```


**Returns**

[DisplayUnitType](../displayunittype/)

### setDisplayUnit(DisplayUnitType) {#setDisplayUnit-displayunittype-}

Represents the unit label for the specified axis.

```javascript
setDisplayUnit(value: DisplayUnitType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DisplayUnitType](../displayunittype/) | The value to set. |

### getCustomUnit() {#getCustomUnit--}

Specifies a custom value for the display unit.

```javascript
getCustomUnit() : number;
```


### setCustomUnit(number) {#setCustomUnit-number-}

Specifies a custom value for the display unit.

```javascript
setCustomUnit(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getDisplayUnitLabel() {#getDisplayUnitLabel--}

Represents a unit label on an axis in the specified chart. Unit labels are useful for charting large values— for example, in the millions or billions.

```javascript
getDisplayUnitLabel() : DisplayUnitLabel;
```


**Returns**

[DisplayUnitLabel](../displayunitlabel/)

### isDisplayUnitLabelShown() {#isDisplayUnitLabelShown--}

Represents if the display unit label is shown on the specified axis.

```javascript
isDisplayUnitLabelShown() : boolean;
```


**Remarks**

The default value is True.

### setIsDisplayUnitLabelShown(boolean) {#setIsDisplayUnitLabelShown-boolean-}

Represents if the display unit label is shown on the specified axis.

```javascript
setIsDisplayUnitLabelShown(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is True.

### getTitle() {#getTitle--}

Gets the axis' title.

```javascript
getTitle() : Title;
```


**Returns**

[Title](../title/)

### getCategoryType() {#getCategoryType--}

Represents the category axis type.

```javascript
getCategoryType() : CategoryType;
```


**Returns**

[CategoryType](../categorytype/)

### setCategoryType(CategoryType) {#setCategoryType-categorytype-}

Represents the category axis type.

```javascript
setCategoryType(value: CategoryType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CategoryType](../categorytype/) | The value to set. |

### getBaseUnitScale() {#getBaseUnitScale--}

Represents the base unit scale for the category axis.

```javascript
getBaseUnitScale() : TimeUnit;
```


**Returns**

[TimeUnit](../timeunit/)

**Remarks**

Setting this property only takes effect when the CategoryType property is set to TimeScale.

### setBaseUnitScale(TimeUnit) {#setBaseUnitScale-timeunit-}

Represents the base unit scale for the category axis.

```javascript
setBaseUnitScale(value: TimeUnit) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TimeUnit](../timeunit/) | The value to set. |

**Remarks**

Setting this property only takes effect when the CategoryType property is set to TimeScale.

### getMajorUnitScale() {#getMajorUnitScale--}

Represents the major unit scale for the category axis.

```javascript
getMajorUnitScale() : TimeUnit;
```


**Returns**

[TimeUnit](../timeunit/)

### setMajorUnitScale(TimeUnit) {#setMajorUnitScale-timeunit-}

Represents the major unit scale for the category axis.

```javascript
setMajorUnitScale(value: TimeUnit) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TimeUnit](../timeunit/) | The value to set. |

### getMinorUnitScale() {#getMinorUnitScale--}

Represents the major unit scale for the category axis.

```javascript
getMinorUnitScale() : TimeUnit;
```


**Returns**

[TimeUnit](../timeunit/)

### setMinorUnitScale(TimeUnit) {#setMinorUnitScale-timeunit-}

Represents the major unit scale for the category axis.

```javascript
setMinorUnitScale(value: TimeUnit) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TimeUnit](../timeunit/) | The value to set. |

### isVisible() {#isVisible--}

Represents if the axis is visible.

```javascript
isVisible() : boolean;
```


### setIsVisible(boolean) {#setIsVisible-boolean-}

Represents if the axis is visible.

```javascript
setIsVisible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMajorGridLines() {#getMajorGridLines--}

Represents major gridlines on a chart axis.

```javascript
getMajorGridLines() : Line;
```


**Returns**

[Line](../line/)

### getMinorGridLines() {#getMinorGridLines--}

Represents minor gridlines on a chart axis.

```javascript
getMinorGridLines() : Line;
```


**Returns**

[Line](../line/)

### getHasMultiLevelLabels() {#getHasMultiLevelLabels--}

Indicates whether the labels shall be shown as multi level.

```javascript
getHasMultiLevelLabels() : boolean;
```


**Remarks**

Only valid for category axis.

### setHasMultiLevelLabels(boolean) {#setHasMultiLevelLabels-boolean-}

Indicates whether the labels shall be shown as multi level.

```javascript
setHasMultiLevelLabels(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only valid for category axis.

### getBins() {#getBins--}

Represents bins on a chart(Histogram/Pareto) axis

```javascript
getBins() : AxisBins;
```


**Returns**

[AxisBins](../axisbins/)

### getAxisTexts() {#getAxisTexts--}

Gets the labels of the axis after call Chart.Calculate() method.

```javascript
getAxisTexts() : string[];
```


**Returns**

string[]

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



