---
title: BorderCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates a collection of Border.border objects.
type: docs
url: /nodejs-cpp/bordercollection/
---

## BorderCollection class

Encapsulates a collection of [Border](./border/) objects.

```javascript
class BorderCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(BorderType)](#get-bordertype-)| Gets the [Border](./border/) element at the specified index. |
| [getDiagonalColor()](#getDiagonalColor--)| Gets or sets the [System.Drawing.Color](./system.drawing.color/) of Diagonal lines. |
| [setDiagonalColor(Color)](#setDiagonalColor-color-)| Gets or sets the [System.Drawing.Color](./system.drawing.color/) of Diagonal lines. |
| [getDiagonalStyle()](#getDiagonalStyle--)| Gets or sets the style of Diagonal lines. |
| [setDiagonalStyle(CellBorderType)](#setDiagonalStyle-cellbordertype-)| Gets or sets the style of Diagonal lines. |
| [setColor(Color)](#setColor-color-)| Sets the [System.Drawing.Color](./system.drawing.color/) of all borders in the collection. |
| [setStyle(CellBorderType)](#setStyle-cellbordertype-)| Sets the style of all borders of the collection. |


### get(BorderType) {#get-bordertype-}

Gets the [Border](./border/) element at the specified index.

```javascript
get(borderType: BorderType) : Border;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderType | [BorderType](./bordertype/) | The border to be retrieved. |

**Returns**

The element at the specified index.

### getDiagonalColor() {#getDiagonalColor--}

Gets or sets the [System.Drawing.Color](./system.drawing.color/) of Diagonal lines.

```javascript
getDiagonalColor() : Color;
```


**Returns**

[Color](./color/)

### setDiagonalColor(Color) {#setDiagonalColor-color-}

Gets or sets the [System.Drawing.Color](./system.drawing.color/) of Diagonal lines.

```javascript
setDiagonalColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](./color/) | The value to set. |

### getDiagonalStyle() {#getDiagonalStyle--}

Gets or sets the style of Diagonal lines.

```javascript
getDiagonalStyle() : CellBorderType;
```


**Returns**

[CellBorderType](./cellbordertype/)

### setDiagonalStyle(CellBorderType) {#setDiagonalStyle-cellbordertype-}

Gets or sets the style of Diagonal lines.

```javascript
setDiagonalStyle(value: CellBorderType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellBorderType](./cellbordertype/) | The value to set. |

### setColor(Color) {#setColor-color-}

Sets the [System.Drawing.Color](./system.drawing.color/) of all borders in the collection.

```javascript
setColor(color: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color | [Color](./color/) | Borders' [System.Drawing.Color](./system.drawing.color/). |

### setStyle(CellBorderType) {#setStyle-cellbordertype-}

Sets the style of all borders of the collection.

```javascript
setStyle(style: CellBorderType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [CellBorderType](./cellbordertype/) | Borders' style |


