---
title: BorderCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates a collection of Border..border objects.
type: docs
url: /ru/javascript-cpp/bordercollection/
---

## BorderCollection class

Encapsulates a collection of [Border](../border/) objects.

```javascript
class BorderCollection;
```


### Example
```javascript
const { Workbook, BorderType, CellBorderType, Color, SaveFormat } = AsposeCells;

//Создание объекта Workbook
var workbook = new Workbook();
//Получение ссылки на только что добавленный лист, передавая его индекс листа
var worksheet = workbook.worksheets.get(0);
//Доступ к ячейке "A1" листа
var cell = worksheet.cells.get("A1");
//Добавление некоторого значения в ячейку "A1"
cell.putValue("Visit Aspose!");
//Получить объект стиля из ячейки
var style = cell.getStyle();
//Установка стиля линии верхней границы
style.borders.get(BorderType.TopBorder).lineStyle = CellBorderType.Thick;
//Установка цвета верхней границы
style.borders.get(BorderType.TopBorder).color = Color.Black;
//Установка стиля линии нижней границы
style.borders.get(BorderType.BottomBorder).lineStyle = CellBorderType.Thick;
//Установка цвета нижней границы
style.borders.get(BorderType.BottomBorder).color = Color.Black;
//Установка стиля линии левой границы
style.borders.get(BorderType.LeftBorder).lineStyle = CellBorderType.Thick;
//Установка цвета левой границы
style.borders.get(BorderType.LeftBorder).color = Color.Black;
//Установка стиля линии правой границы
style.borders.get(BorderType.RightBorder).lineStyle = CellBorderType.Thick;
//Установка цвета правой границы
style.borders.get(BorderType.RightBorder).color = Color.Black;
//Установить объект стиля в ячейку
cell.setStyle(style);

//Сохранение файла Excel
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


