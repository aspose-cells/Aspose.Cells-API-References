---
title: Border
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents the cell border.
type: docs
url: /nodejs-cpp/border/
---

## Border class

Encapsulates the object that represents the cell border.

```javascript
class Border;
```


### Example
```javascript
const { Workbook, BorderType, CellBorderType, Color } = require("aspose.cells.node");

var workbook = new Workbook();
var worksheet = workbook.getWorksheets().get(0);
var cell = worksheet.getCells().get(0, 0);
var style = workbook.createStyle();
//Set top border style and color
var border = style.getBorders().get(BorderType.TopBorder);
border.setLineStyle(CellBorderType.Medium);
border.setColor(Color.Red);
cell.setStyle(style);
```
## Methods

| Method | Description |
| --- | --- |
| [getThemeColor()](#getThemeColor--)| Gets and sets the theme color of the border. |
| [setThemeColor(ThemeColor)](#setThemeColor-themecolor-)| Gets and sets the theme color of the border. |
| [getColor()](#getColor--)| Gets or sets the [Color](../color/) of the border. |
| [setColor(Color)](#setColor-color-)| Gets or sets the [Color](../color/) of the border. |
| [getArgbColor()](#getArgbColor--)| Gets and sets the color with a 32-bit ARGB value. |
| [setArgbColor(number)](#setArgbColor-number-)| Gets and sets the color with a 32-bit ARGB value. |
| [getLineStyle()](#getLineStyle--)| Gets or sets the cell border type. |
| [setLineStyle(CellBorderType)](#setLineStyle-cellbordertype-)| Gets or sets the cell border type. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getThemeColor() {#getThemeColor--}

Gets and sets the theme color of the border.

```javascript
getThemeColor() : ThemeColor;
```


**Returns**

[ThemeColor](../themecolor/)

### setThemeColor(ThemeColor) {#setThemeColor-themecolor-}

Gets and sets the theme color of the border.

```javascript
setThemeColor(value: ThemeColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../themecolor/) | The value to set. |

### getColor() {#getColor--}

Gets or sets the [Color](../color/) of the border.

```javascript
getColor() : Color;
```


**Returns**

[Color](../color/)

### setColor(Color) {#setColor-color-}

Gets or sets the [Color](../color/) of the border.

```javascript
setColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

### getArgbColor() {#getArgbColor--}

Gets and sets the color with a 32-bit ARGB value.

```javascript
getArgbColor() : number;
```


### setArgbColor(number) {#setArgbColor-number-}

Gets and sets the color with a 32-bit ARGB value.

```javascript
setArgbColor(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getLineStyle() {#getLineStyle--}

Gets or sets the cell border type.

```javascript
getLineStyle() : CellBorderType;
```


**Returns**

[CellBorderType](../cellbordertype/)

### setLineStyle(CellBorderType) {#setLineStyle-cellbordertype-}

Gets or sets the cell border type.

```javascript
setLineStyle(value: CellBorderType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellBorderType](../cellbordertype/) | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



