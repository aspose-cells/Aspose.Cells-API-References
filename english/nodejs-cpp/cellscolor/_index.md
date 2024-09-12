---
title: CellsColor
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents all types of color.
type: docs
url: /nodejs-cpp/cellscolor/
---

## CellsColor class

Represents all types of color.

```javascript
class CellsColor;
```


## Methods

| Method | Description |
| --- | --- |
| [isShapeColor()](#isShapeColor--)| Gets and set the color which should apply to cell or shape. |
| [setIsShapeColor(boolean)](#setIsShapeColor-boolean-)| Gets and set the color which should apply to cell or shape. |
| [getType()](#getType--)| The color type. |
| [getThemeColor()](#getThemeColor--)| Gets the theme color. Only applies for theme color type. |
| [setThemeColor(ThemeColor)](#setThemeColor-themecolor-)| Gets the theme color. Only applies for theme color type. |
| [getColorIndex()](#getColorIndex--)| Gets and sets the color index in the color palette. Only applies of indexed color. |
| [setColorIndex(number)](#setColorIndex-number-)| Gets and sets the color index in the color palette. Only applies of indexed color. |
| [getColor()](#getColor--)| Gets and sets the RGB color. |
| [setColor(Color)](#setColor-color-)| Gets and sets the RGB color. |
| [getArgb()](#getArgb--)| Gets and sets the color from a 32-bit ARGB value. |
| [setArgb(number)](#setArgb-number-)| Gets and sets the color from a 32-bit ARGB value. |
| [getTransparency()](#getTransparency--)| Gets and sets transparency as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| Gets and sets transparency as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTintOfShapeColor(number)](#setTintOfShapeColor-number-)| Set the tint of the shape color |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### isShapeColor() {#isShapeColor--}

Gets and set the color which should apply to cell or shape.

```javascript
isShapeColor() : boolean;
```


**Remarks**

The expression of the color of the cell and the shape is different. For example: the theme color with same tint value will be not same in the cell and the shape.

### setIsShapeColor(boolean) {#setIsShapeColor-boolean-}

Gets and set the color which should apply to cell or shape.

```javascript
setIsShapeColor(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The expression of the color of the cell and the shape is different. For example: the theme color with same tint value will be not same in the cell and the shape.

### getType() {#getType--}

The color type.

```javascript
getType() : ColorType;
```


**Returns**

[ColorType](../colortype/)

### getThemeColor() {#getThemeColor--}

Gets the theme color. Only applies for theme color type.

```javascript
getThemeColor() : ThemeColor;
```


**Returns**

[ThemeColor](../themecolor/)

### setThemeColor(ThemeColor) {#setThemeColor-themecolor-}

Gets the theme color. Only applies for theme color type.

```javascript
setThemeColor(value: ThemeColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../themecolor/) | The value to set. |

### getColorIndex() {#getColorIndex--}

Gets and sets the color index in the color palette. Only applies of indexed color.

```javascript
getColorIndex() : number;
```


### setColorIndex(number) {#setColorIndex-number-}

Gets and sets the color index in the color palette. Only applies of indexed color.

```javascript
setColorIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getColor() {#getColor--}

Gets and sets the RGB color.

```javascript
getColor() : Color;
```


**Returns**

[Color](../color/)

### setColor(Color) {#setColor-color-}

Gets and sets the RGB color.

```javascript
setColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

### getArgb() {#getArgb--}

Gets and sets the color from a 32-bit ARGB value.

```javascript
getArgb() : number;
```


### setArgb(number) {#setArgb-number-}

Gets and sets the color from a 32-bit ARGB value.

```javascript
setArgb(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getTransparency() {#getTransparency--}

Gets and sets transparency as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
getTransparency() : number;
```


### setTransparency(number) {#setTransparency-number-}

Gets and sets transparency as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
setTransparency(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### setTintOfShapeColor(number) {#setTintOfShapeColor-number-}

Set the tint of the shape color

```javascript
setTintOfShapeColor(tint: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tint | number |  |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



