---
title: BorderCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates a collection of Border..border objects.
type: docs
url: /zh/javascript-cpp/bordercollection/
---

## BorderCollection class

Encapsulates a collection of [Border](../border/) objects.

```javascript
class BorderCollection;
```


### Example
```javascript
const { Workbook, BorderType, CellBorderType, Color, SaveFormat } = AsposeCells;

//实例化一个 Workbook 对象
var workbook = new Workbook();
//通过传递工作表索引获取新添加工作表的引用
var worksheet = workbook.worksheets.get(0);
//从工作表访问 "A1" 单元格
var cell = worksheet.cells.get("A1");
//向 "A1" 单元格添加一些值
cell.putValue("Visit Aspose!");
//从单元格获取样式对象
var style = cell.getStyle();
//设置上边框的线型
style.borders.get(BorderType.TopBorder).lineStyle = CellBorderType.Thick;
//设置上边框的颜色
style.borders.get(BorderType.TopBorder).color = Color.Black;
//设置下边框的线型
style.borders.get(BorderType.BottomBorder).lineStyle = CellBorderType.Thick;
//设置下边框的颜色
style.borders.get(BorderType.BottomBorder).color = Color.Black;
//设置左边框的线型
style.borders.get(BorderType.LeftBorder).lineStyle = CellBorderType.Thick;
//设置左边框的颜色
style.borders.get(BorderType.LeftBorder).color = Color.Black;
//设置右边框的线型
style.borders.get(BorderType.RightBorder).lineStyle = CellBorderType.Thick;
//设置右边框的颜色
style.borders.get(BorderType.RightBorder).color = Color.Black;
//将样式对象设置到单元格
cell.setStyle(style);

//保存 Excel 文件
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Properties

| Property | Type | Description |
| --- | --- | --- |
| [isOutline](#isOutline--)| boolean | Indicates if left, right, top, and bottom borders should be applied only to outside borders of a cell range. Default value is true. |
| [diagonalColor](#diagonalColor--)| Color | Gets or sets the [Color](../color/) of Diagonal lines. |
| [diagonalStyle](#diagonalStyle--)| CellBorderType | Gets or sets the style of Diagonal lines. |

## Methods

| Method | Description |
| --- | --- |
| [get(BorderType)](#get-bordertype-)| Gets the [Border](../border/) element at the specified index. |
| [setColor(Color)](#setColor-color-)| Sets the [Color](../color/) of all borders in the collection. |
| [setStyle(CellBorderType)](#setStyle-cellbordertype-)| Sets the style of all borders of the collection. |


### isOutline {#isOutline--}

Indicates if left, right, top, and bottom borders should be applied only to outside borders of a cell range. Default value is true.

```javascript
isOutline : boolean;
```


**Remarks**

Only works when applying to a range for conditional formattings, pivot tables. If false,left, right, top, and bottom will apply to each cell, otherwise only to outside borders of a cell range. If true, please set horizontal and vertical border of inner borders of range for conditional formattings, pivot tables.

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


