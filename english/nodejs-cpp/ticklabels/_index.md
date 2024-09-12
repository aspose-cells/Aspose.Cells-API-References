---
title: TickLabels
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the tickmark labels associated with tick marks on a chart axis.
type: docs
url: /nodejs-cpp/ticklabels/
---

## TickLabels class

Represents the tick-mark labels associated with tick marks on a chart axis.

```javascript
class TickLabels;
```


## Methods

| Method | Description |
| --- | --- |
| [getFont()](#getFont--)| Returns a [Font](../font/) object that represents the font of the specified TickLabels object. |
| [getAutoScaleFont()](#getAutoScaleFont--)| True if the text in the object changes font size when the object size changes. The default value is True. |
| [setAutoScaleFont(boolean)](#setAutoScaleFont-boolean-)| True if the text in the object changes font size when the object size changes. The default value is True. |
| [getBackgroundMode()](#getBackgroundMode--)| Gets and sets the display mode of the background |
| [setBackgroundMode(BackgroundMode)](#setBackgroundMode-backgroundmode-)| Gets and sets the display mode of the background |
| [getRotationAngle()](#getRotationAngle--)| Represents text rotation angle in clockwise. |
| [setRotationAngle(number)](#setRotationAngle-number-)| Represents text rotation angle in clockwise. |
| [isAutomaticRotation()](#isAutomaticRotation--)| Indicates whether the rotation angle is automatic |
| [setIsAutomaticRotation(boolean)](#setIsAutomaticRotation-boolean-)| Indicates whether the rotation angle is automatic |
| [get_NumberFormat()](#get_NumberFormat--)| Represents the format string for the TickLabels object. |
| [setNumberFormat(string)](#setNumberFormat-string-)| Represents the format string for the TickLabels object. |
| [getNumber()](#getNumber--)| Represents the format number for the TickLabels object. |
| [setNumber(number)](#setNumber-number-)| Represents the format number for the TickLabels object. |
| [getNumberFormatLinked()](#getNumberFormatLinked--)| True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells). |
| [setNumberFormatLinked(boolean)](#setNumberFormatLinked-boolean-)| True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells). |
| [getDisplayNumberFormat()](#getDisplayNumberFormat--)| Gets and sets the display number format of tick labels. |
| [getOffset()](#getOffset--)| Gets and sets the distance between the axis labels and the axis line. |
| [setOffset(number)](#setOffset-number-)| Gets and sets the distance between the axis labels and the axis line. |
| [getReadingOrder()](#getReadingOrder--)| Represents text reading order. |
| [setReadingOrder(TextDirectionType)](#setReadingOrder-textdirectiontype-)| Represents text reading order. |
| [getDirectionType()](#getDirectionType--)| Gets and sets the direction of text. |
| [setDirectionType(ChartTextDirectionType)](#setDirectionType-charttextdirectiontype-)| Gets and sets the direction of text. |
| [getTickLabelItems()](#getTickLabelItems--)| Gets the display tick labels of the axis. |
| [getAlignmentType()](#getAlignmentType--)| Gets and sets the text alignment for the tick labels on the axis. |
| [setAlignmentType(TickLabelAlignmentType)](#setAlignmentType-ticklabelalignmenttype-)| Gets and sets the text alignment for the tick labels on the axis. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getFont() {#getFont--}

Returns a [Font](../font/) object that represents the font of the specified TickLabels object.

```javascript
getFont() : Font;
```


**Returns**

[Font](../font/)

### getAutoScaleFont() {#getAutoScaleFont--}

True if the text in the object changes font size when the object size changes. The default value is True.

```javascript
getAutoScaleFont() : boolean;
```


### setAutoScaleFont(boolean) {#setAutoScaleFont-boolean-}

True if the text in the object changes font size when the object size changes. The default value is True.

```javascript
setAutoScaleFont(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getBackgroundMode() {#getBackgroundMode--}

Gets and sets the display mode of the background

```javascript
getBackgroundMode() : BackgroundMode;
```


**Returns**

[BackgroundMode](../backgroundmode/)

### setBackgroundMode(BackgroundMode) {#setBackgroundMode-backgroundmode-}

Gets and sets the display mode of the background

```javascript
setBackgroundMode(value: BackgroundMode) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [BackgroundMode](../backgroundmode/) | The value to set. |

### getRotationAngle() {#getRotationAngle--}

Represents text rotation angle in clockwise.

```javascript
getRotationAngle() : number;
```


**Remarks**

<br>0: Not rotated.</br> <br>255: Top to Bottom.</br> <br>-90: Downward.</br> <br>90: Upward.</br>

### setRotationAngle(number) {#setRotationAngle-number-}

Represents text rotation angle in clockwise.

```javascript
setRotationAngle(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

<br>0: Not rotated.</br> <br>255: Top to Bottom.</br> <br>-90: Downward.</br> <br>90: Upward.</br>

### isAutomaticRotation() {#isAutomaticRotation--}

Indicates whether the rotation angle is automatic

```javascript
isAutomaticRotation() : boolean;
```


### setIsAutomaticRotation(boolean) {#setIsAutomaticRotation-boolean-}

Indicates whether the rotation angle is automatic

```javascript
setIsAutomaticRotation(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### get_NumberFormat() {#get_NumberFormat--}

Represents the format string for the TickLabels object.

```javascript
get_NumberFormat() : string;
```


**Remarks**

The formatting string is same as a custom format string setting to a cell. For example, "$0".

### setNumberFormat(string) {#setNumberFormat-string-}

Represents the format string for the TickLabels object.

```javascript
setNumberFormat(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

The formatting string is same as a custom format string setting to a cell. For example, "$0".

### getNumber() {#getNumber--}

Represents the format number for the TickLabels object.

```javascript
getNumber() : number;
```


### setNumber(number) {#setNumber-number-}

Represents the format number for the TickLabels object.

```javascript
setNumber(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getNumberFormatLinked() {#getNumberFormatLinked--}

True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells).

```javascript
getNumberFormatLinked() : boolean;
```


### setNumberFormatLinked(boolean) {#setNumberFormatLinked-boolean-}

True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells).

```javascript
setNumberFormatLinked(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDisplayNumberFormat() {#getDisplayNumberFormat--}

Gets and sets the display number format of tick labels.

```javascript
getDisplayNumberFormat() : string;
```


### getOffset() {#getOffset--}

Gets and sets the distance between the axis labels and the axis line.

```javascript
getOffset() : number;
```


**Remarks**

The default distance is 100 percent, which represents the default spacing between the axis labels and the axis line. The value can be an integer percentage from 0 through 1000, relative to the axis label’s font size.

### setOffset(number) {#setOffset-number-}

Gets and sets the distance between the axis labels and the axis line.

```javascript
setOffset(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The default distance is 100 percent, which represents the default spacing between the axis labels and the axis line. The value can be an integer percentage from 0 through 1000, relative to the axis label’s font size.

### getReadingOrder() {#getReadingOrder--}

Represents text reading order.

```javascript
getReadingOrder() : TextDirectionType;
```


**Returns**

[TextDirectionType](../textdirectiontype/)

### setReadingOrder(TextDirectionType) {#setReadingOrder-textdirectiontype-}

Represents text reading order.

```javascript
setReadingOrder(value: TextDirectionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextDirectionType](../textdirectiontype/) | The value to set. |

### getDirectionType() {#getDirectionType--}

Gets and sets the direction of text.

```javascript
getDirectionType() : ChartTextDirectionType;
```


**Returns**

[ChartTextDirectionType](../charttextdirectiontype/)

### setDirectionType(ChartTextDirectionType) {#setDirectionType-charttextdirectiontype-}

Gets and sets the direction of text.

```javascript
setDirectionType(value: ChartTextDirectionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ChartTextDirectionType](../charttextdirectiontype/) | The value to set. |

### getTickLabelItems() {#getTickLabelItems--}

Gets the display tick labels of the axis.

```javascript
getTickLabelItems() : TickLabelItem[];
```


**Returns**

[TickLabelItem](../ticklabelitem/)[]

**Remarks**

Only available after calling [Chart.Calculate()](../chart.calculate()/) method.

### getAlignmentType() {#getAlignmentType--}

Gets and sets the text alignment for the tick labels on the axis.

```javascript
getAlignmentType() : TickLabelAlignmentType;
```


**Returns**

[TickLabelAlignmentType](../ticklabelalignmenttype/)

### setAlignmentType(TickLabelAlignmentType) {#setAlignmentType-ticklabelalignmenttype-}

Gets and sets the text alignment for the tick labels on the axis.

```javascript
setAlignmentType(value: TickLabelAlignmentType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TickLabelAlignmentType](../ticklabelalignmenttype/) | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



