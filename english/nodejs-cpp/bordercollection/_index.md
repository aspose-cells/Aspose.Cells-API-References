---
title: BorderCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates a collection of Border..border objects.
type: docs
url: /nodejs-cpp/bordercollection/
---

## BorderCollection class

Encapsulates a collection of [Border](../border/) objects.

```javascript
class BorderCollection;
```


### Example
```javascript
const { Workbook, BorderType, CellBorderType, Color } = require("aspose.cells.node");

//Instantiating a Workbook object
var workbook = new Workbook();
//Obtaining the reference of the newly added worksheet by passing its sheet index
var worksheet = workbook.getWorksheets().get(0);
//Accessing the "A1" cell from the worksheet
var cell = worksheet.getCells().get("A1");
//Adding some value to the "A1" cell
cell.putValue("Visit Aspose!");
//Get style object from cell
var style = cell.getStyle();
//Setting the line style of the top border
style.getBorders().get(BorderType.TopBorder).setLineStyle(CellBorderType.Thick);
//Setting the color of the top border
var black = new Color(0, 0, 0);
style.getBorders().get(BorderType.TopBorder).setColor(black);
//Setting the line style of the bottom border
style.getBorders().get(BorderType.BottomBorder).setLineStyle(CellBorderType.Thick);
//Setting the color of the bottom border
style.getBorders().get(BorderType.BottomBorder).setColor(black);
//Setting the line style of the left border
style.getBorders().get(BorderType.LeftBorder).setLineStyle(CellBorderType.Thick);
//Setting the color of the left border
style.getBorders().get(BorderType.LeftBorder).setColor(black);
//Setting the line style of the right border
style.getBorders().get(BorderType.RightBorder).setLineStyle(CellBorderType.Thick);
//Setting the color of the right border
style.getBorders().get(BorderType.RightBorder).setColor(black);
//Set style object to cell
cell.setStyle(style);

//Saving the Excel file
workbook.save("output/BorderCollection.xls");
```
## Methods

| Method | Description |
| --- | --- |
| [get(BorderType)](#get-bordertype-)| Gets the [Border](../border/) element at the specified index. |
| [getDiagonalColor()](#getDiagonalColor--)| Gets or sets the [Color](../color/) of Diagonal lines. |
| [setDiagonalColor(Color)](#setDiagonalColor-color-)| Gets or sets the [Color](../color/) of Diagonal lines. |
| [getDiagonalStyle()](#getDiagonalStyle--)| Gets or sets the style of Diagonal lines. |
| [setDiagonalStyle(CellBorderType)](#setDiagonalStyle-cellbordertype-)| Gets or sets the style of Diagonal lines. |
| [setColor(Color)](#setColor-color-)| Sets the [Color](../color/) of all borders in the collection. |
| [setStyle(CellBorderType)](#setStyle-cellbordertype-)| Sets the style of all borders of the collection. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### get(BorderType) {#get-bordertype-}

Gets the [Border](../border/) element at the specified index.

```javascript
get(borderType: BorderType) : Border;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderType | [BorderType](../bordertype/) | The border to be retrieved. |

**Returns**

The element at the specified index.

### getDiagonalColor() {#getDiagonalColor--}

Gets or sets the [Color](../color/) of Diagonal lines.

```javascript
getDiagonalColor() : Color;
```


**Returns**

[Color](../color/)

### setDiagonalColor(Color) {#setDiagonalColor-color-}

Gets or sets the [Color](../color/) of Diagonal lines.

```javascript
setDiagonalColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

### getDiagonalStyle() {#getDiagonalStyle--}

Gets or sets the style of Diagonal lines.

```javascript
getDiagonalStyle() : CellBorderType;
```


**Returns**

[CellBorderType](../cellbordertype/)

### setDiagonalStyle(CellBorderType) {#setDiagonalStyle-cellbordertype-}

Gets or sets the style of Diagonal lines.

```javascript
setDiagonalStyle(value: CellBorderType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellBorderType](../cellbordertype/) | The value to set. |

### setColor(Color) {#setColor-color-}

Sets the [Color](../color/) of all borders in the collection.

```javascript
setColor(color: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color | [Color](../color/) | Borders' [Color](../color/). |

### setStyle(CellBorderType) {#setStyle-cellbordertype-}

Sets the style of all borders of the collection.

```javascript
setStyle(style: CellBorderType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [CellBorderType](../cellbordertype/) | Borders' style |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



