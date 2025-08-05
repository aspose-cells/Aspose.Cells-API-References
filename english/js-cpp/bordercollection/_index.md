﻿---
title: BorderCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates a collection of Border..border objects.
type: docs
url: /js-cpp/bordercollection/
---

## BorderCollection class

Encapsulates a collection of [Border](../border/) objects.

```javascript
class BorderCollection;
```


### Example
```javascript
const { Workbook, BorderType, CellBorderType, Color, SaveFormat } = AsposeCells;

//Instantiating a Workbook object
var workbook = new Workbook();
//Obtaining the reference of the newly added worksheet by passing its sheet index
var worksheet = workbook.worksheets.get(0);
//Accessing the "A1" cell from the worksheet
var cell = worksheet.cells.get("A1");
//Adding some value to the "A1" cell
cell.putValue("Visit Aspose!");
//Get style object from cell
var style = cell.getStyle();
//Setting the line style of the top border
style.borders.get(BorderType.TopBorder).lineStyle = CellBorderType.Thick;
//Setting the color of the top border
style.borders.get(BorderType.TopBorder).color = Color.Black;
//Setting the line style of the bottom border
style.borders.get(BorderType.BottomBorder).lineStyle = CellBorderType.Thick;
//Setting the color of the bottom border
style.borders.get(BorderType.BottomBorder).color = Color.Black;
//Setting the line style of the left border
style.borders.get(BorderType.LeftBorder).lineStyle = CellBorderType.Thick;
//Setting the color of the left border
style.borders.get(BorderType.LeftBorder).color = Color.Black;
//Setting the line style of the right border
style.borders.get(BorderType.RightBorder).lineStyle = CellBorderType.Thick;
//Setting the color of the right border
style.borders.get(BorderType.RightBorder).color = Color.Black;
//Set style object to cell
cell.setStyle(style);

//Saving the Excel file
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Properties

| Property | Type | Description |
| --- | --- | --- |
| [diagonalColor](#diagonalColor--)| Color | Gets or sets the [Color](../color/) of Diagonal lines. |
| [diagonalStyle](#diagonalStyle--)| CellBorderType | Gets or sets the style of Diagonal lines. |

## Methods

| Method | Description |
| --- | --- |
| [get(BorderType)](#get-bordertype-)| Gets the [Border](../border/) element at the specified index. |
| [setColor(Color)](#setColor-color-)| Sets the [Color](../color/) of all borders in the collection. |
| [setStyle(CellBorderType)](#setStyle-cellbordertype-)| Sets the style of all borders of the collection. |


### diagonalColor {#diagonalColor--}

Gets or sets the [Color](../color/) of Diagonal lines.

```javascript
diagonalColor : Color;
```


### diagonalStyle {#diagonalStyle--}

Gets or sets the style of Diagonal lines.

```javascript
diagonalStyle : CellBorderType;
```


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


