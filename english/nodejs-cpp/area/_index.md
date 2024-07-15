---
title: Area
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents an area format.
type: docs
url: /nodejs-cpp/area/
---

## Area class

Encapsulates the object that represents an area format.

```javascript
class Area;
```


## Methods

| Method | Description |
| --- | --- |
| [getBackgroundColor()](#getBackgroundColor--)| Gets or sets the background [System.Drawing.Color](../system.drawing.color/) of the [System.Drawing.Color](../system.drawing.color/). |
| [setBackgroundColor(Color)](#setBackgroundColor-color-)| Gets or sets the background [System.Drawing.Color](../system.drawing.color/) of the [System.Drawing.Color](../system.drawing.color/). |
| [getForegroundColor()](#getForegroundColor--)| Gets or sets the foreground [System.Drawing.Color](../system.drawing.color/). |
| [setForegroundColor(Color)](#setForegroundColor-color-)| Gets or sets the foreground [System.Drawing.Color](../system.drawing.color/). |
| [getFormatting()](#getFormatting--)| Represents the formatting of the area. |
| [setFormatting(FormattingType)](#setFormatting-formattingtype-)| Represents the formatting of the area. |
| [getInvertIfNegative()](#getInvertIfNegative--)| If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [setInvertIfNegative(boolean)](#setInvertIfNegative-boolean-)| If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [getFillFormat()](#getFillFormat--)| Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape. |
| [getTransparency()](#getTransparency--)| Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |


### getBackgroundColor() {#getBackgroundColor--}

Gets or sets the background [System.Drawing.Color](../system.drawing.color/) of the [System.Drawing.Color](../system.drawing.color/).

```javascript
getBackgroundColor() : Color;
```


**Returns**

[Color](../color/)

### setBackgroundColor(Color) {#setBackgroundColor-color-}

Gets or sets the background [System.Drawing.Color](../system.drawing.color/) of the [System.Drawing.Color](../system.drawing.color/).

```javascript
setBackgroundColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

### getForegroundColor() {#getForegroundColor--}

Gets or sets the foreground [System.Drawing.Color](../system.drawing.color/).

```javascript
getForegroundColor() : Color;
```


**Returns**

[Color](../color/)

### setForegroundColor(Color) {#setForegroundColor-color-}

Gets or sets the foreground [System.Drawing.Color](../system.drawing.color/).

```javascript
setForegroundColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

### getFormatting() {#getFormatting--}

Represents the formatting of the area.

```javascript
getFormatting() : FormattingType;
```


**Returns**

[FormattingType](../formattingtype/)

### setFormatting(FormattingType) {#setFormatting-formattingtype-}

Represents the formatting of the area.

```javascript
setFormatting(value: FormattingType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FormattingType](../formattingtype/) | The value to set. |

### getInvertIfNegative() {#getInvertIfNegative--}

If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```javascript
getInvertIfNegative() : boolean;
```


### setInvertIfNegative(boolean) {#setInvertIfNegative-boolean-}

If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```javascript
setInvertIfNegative(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFillFormat() {#getFillFormat--}

Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape.

```javascript
getFillFormat() : FillFormat;
```


**Returns**

[FillFormat](../fillformat/)

### getTransparency() {#getTransparency--}

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
getTransparency() : number;
```


### setTransparency(number) {#setTransparency-number-}

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
setTransparency(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |


