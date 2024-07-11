---
title: DataBar
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Describe the DataBar conditional formatting rule. This conditional formatting rule displays a gradated data bar in the range of cells.
type: docs
url: /nodejs-cpp/databar/
---

## DataBar class

Describe the DataBar conditional formatting rule. This conditional formatting rule displays a gradated data bar in the range of cells.

```javascript
class DataBar;
```


## Methods

| Method | Description |
| --- | --- |
| [getAxisColor()](#getAxisColor--)| Gets the color of the axis for cells with conditional formatting as data bars. |
| [setAxisColor(Color)](#setAxisColor-color-)| Gets the color of the axis for cells with conditional formatting as data bars. |
| [getAxisPosition()](#getAxisPosition--)| Gets or sets the position of the axis of the data bars specified by a conditional formatting rule. |
| [setAxisPosition(DataBarAxisPosition)](#setAxisPosition-databaraxisposition-)| Gets or sets the position of the axis of the data bars specified by a conditional formatting rule. |
| [getBarFillType()](#getBarFillType--)| Gets or sets how a data bar is filled with color. |
| [setBarFillType(DataBarFillType)](#setBarFillType-databarfilltype-)| Gets or sets how a data bar is filled with color. |
| [getDirection()](#getDirection--)| Gets or sets the direction the databar is displayed. |
| [setDirection(TextDirectionType)](#setDirection-textdirectiontype-)| Gets or sets the direction the databar is displayed. |
| [getBarBorder()](#getBarBorder--)| Gets an object that specifies the border of a data bar. |
| [getNegativeBarFormat()](#getNegativeBarFormat--)| Gets the NegativeBarFormat object associated with a data bar conditional formatting rule. |
| [getMinCfvo()](#getMinCfvo--)| Get or set this DataBar's min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it. |
| [getMaxCfvo()](#getMaxCfvo--)| Get or set this DataBar's max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it. |
| [getColor()](#getColor--)| Get or set this DataBar's Color. |
| [setColor(Color)](#setColor-color-)| Get or set this DataBar's Color. |
| [getMinLength()](#getMinLength--)| Represents the min length of data bar . |
| [setMinLength(number)](#setMinLength-number-)| Represents the min length of data bar . |
| [getMaxLength()](#getMaxLength--)| Represents the max length of data bar . |
| [setMaxLength(number)](#setMaxLength-number-)| Represents the max length of data bar . |
| [getShowValue()](#getShowValue--)| Get or set the flag indicating whether to show the values of the cells on which this data bar is applied. Default value is true. |
| [setShowValue(boolean)](#setShowValue-boolean-)| Get or set the flag indicating whether to show the values of the cells on which this data bar is applied. Default value is true. |
| [toImage(Cell, ImageOrPrintOptions)](#toImage-cell-imageorprintoptions-)| Render data bar in cell to image byte array. |


### getAxisColor() {#getAxisColor--}

Gets the color of the axis for cells with conditional formatting as data bars.

```javascript
getAxisColor() : Color;
```


**Returns**

[Color](./color/)

### setAxisColor(Color) {#setAxisColor-color-}

Gets the color of the axis for cells with conditional formatting as data bars.

```javascript
setAxisColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](./color/) | The value to set. |

### getAxisPosition() {#getAxisPosition--}

Gets or sets the position of the axis of the data bars specified by a conditional formatting rule.

```javascript
getAxisPosition() : DataBarAxisPosition;
```


**Returns**

[DataBarAxisPosition](./databaraxisposition/)

### setAxisPosition(DataBarAxisPosition) {#setAxisPosition-databaraxisposition-}

Gets or sets the position of the axis of the data bars specified by a conditional formatting rule.

```javascript
setAxisPosition(value: DataBarAxisPosition) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DataBarAxisPosition](./databaraxisposition/) | The value to set. |

### getBarFillType() {#getBarFillType--}

Gets or sets how a data bar is filled with color.

```javascript
getBarFillType() : DataBarFillType;
```


**Returns**

[DataBarFillType](./databarfilltype/)

### setBarFillType(DataBarFillType) {#setBarFillType-databarfilltype-}

Gets or sets how a data bar is filled with color.

```javascript
setBarFillType(value: DataBarFillType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DataBarFillType](./databarfilltype/) | The value to set. |

### getDirection() {#getDirection--}

Gets or sets the direction the databar is displayed.

```javascript
getDirection() : TextDirectionType;
```


**Returns**

[TextDirectionType](./textdirectiontype/)

### setDirection(TextDirectionType) {#setDirection-textdirectiontype-}

Gets or sets the direction the databar is displayed.

```javascript
setDirection(value: TextDirectionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextDirectionType](./textdirectiontype/) | The value to set. |

### getBarBorder() {#getBarBorder--}

Gets an object that specifies the border of a data bar.

```javascript
getBarBorder() : DataBarBorder;
```


**Returns**

[DataBarBorder](./databarborder/)

### getNegativeBarFormat() {#getNegativeBarFormat--}

Gets the NegativeBarFormat object associated with a data bar conditional formatting rule.

```javascript
getNegativeBarFormat() : NegativeBarFormat;
```


**Returns**

[NegativeBarFormat](./negativebarformat/)

### getMinCfvo() {#getMinCfvo--}

Get or set this DataBar's min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it.

```javascript
getMinCfvo() : ConditionalFormattingValue;
```


**Returns**

[ConditionalFormattingValue](./conditionalformattingvalue/)

### getMaxCfvo() {#getMaxCfvo--}

Get or set this DataBar's max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it.

```javascript
getMaxCfvo() : ConditionalFormattingValue;
```


**Returns**

[ConditionalFormattingValue](./conditionalformattingvalue/)

### getColor() {#getColor--}

Get or set this DataBar's Color.

```javascript
getColor() : Color;
```


**Returns**

[Color](./color/)

### setColor(Color) {#setColor-color-}

Get or set this DataBar's Color.

```javascript
setColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](./color/) | The value to set. |

### getMinLength() {#getMinLength--}

Represents the min length of data bar .

```javascript
getMinLength() : number;
```


### setMinLength(number) {#setMinLength-number-}

Represents the min length of data bar .

```javascript
setMinLength(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getMaxLength() {#getMaxLength--}

Represents the max length of data bar .

```javascript
getMaxLength() : number;
```


### setMaxLength(number) {#setMaxLength-number-}

Represents the max length of data bar .

```javascript
setMaxLength(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getShowValue() {#getShowValue--}

Get or set the flag indicating whether to show the values of the cells on which this data bar is applied. Default value is true.

```javascript
getShowValue() : boolean;
```


### setShowValue(boolean) {#setShowValue-boolean-}

Get or set the flag indicating whether to show the values of the cells on which this data bar is applied. Default value is true.

```javascript
setShowValue(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### toImage(Cell, ImageOrPrintOptions) {#toImage-cell-imageorprintoptions-}

Render data bar in cell to image byte array.

```javascript
toImage(cell: Cell, imgOpts: ImageOrPrintOptions) : number[];
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cell | [Cell](./cell/) | Indicate the data bar in which cell to be rendered |
| imgOpts | [ImageOrPrintOptions](./imageorprintoptions/) | ImageOrPrintOptions contains some property of output image |

**Returns**

number[]


