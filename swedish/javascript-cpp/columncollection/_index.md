---
title: ColumnCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Collection of the Column..column objects that represent the individual columnsettings in a worksheet. The Column object only represents the settings such as column width styles .etc. for the whole column has nothing to do with the fact that there are nonempty cellsdata or not in corresponding column. And the Count of this collection only represents the count Column objects that have been instantiated in this collection has nothing to do with the fact that there are nonempty cellsdata or not in the worksheet.
type: docs
url: /sv/javascript-cpp/columncollection/
---

## ColumnCollection class

Collection of the [Column](../column/) objects that represent the individual column(setting)s in a worksheet. The Column object only represents the settings such as column width, styles, .etc. for the whole column, has nothing to do with the fact that there are non-empty cells(data) or not in corresponding column. And the "Count" of this collection only represents the count Column objects that have been instantiated in this collection, has nothing to do with the fact that there are non-empty cells(data) or not in the worksheet.

```javascript
class ColumnCollection;
```


### Example
```javascript
const { Workbook, Color, BackgroundType, StyleFlag, SaveFormat } = AsposeCells;

//Instansiering av ett Workbook-objekt
var workbook = new Workbook();
//Hämtar referensen till det första kalkylbladet
var worksheet = workbook.worksheets.get(0);
//Lägg till ny stil i arbetsboken
var style = workbook.createStyle();
//Ställer in bakgrundsfärgen till blå
style.foregroundColor = Color.Blue;
//ställer in bakgrundsmönster
style.pattern = BackgroundType.Solid;
//Ny stilflagga
var styleFlag = new StyleFlag();
//Ange alla stilar
styleFlag.all = true;

//Ändra standardbredden för de första tio kolumnerna
for (var i = 0; i < 10; i++) {
    worksheet.cells.columns.get(i).width = 20;
}

//Hämta kolumnen med icke-standardformatering
var columns = worksheet.cells.columns;
var count = columns.count;
for (var i = 0; i < count; i++) {
    var column = columns.getColumnByIndex(i);
    //Applicera stil på de första tio kolumnerna
    column.applyStyle(style, styleFlag);
}

//Sparar Excel-filen
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets a [Column](../column/) object by column index. The Column object of given column index will be instantiated if it does not exist before. |
| [getColumnByIndex(number)](#getColumnByIndex-number-)| Gets the [Column](../column/) object by the position in the list. |


### get(number) {#get-number-}

Gets a [Column](../column/) object by column index. The Column object of given column index will be instantiated if it does not exist before.

```javascript
get(columnIndex: number) : Column;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number |  |

**Returns**

[Column](../column/)

### getColumnByIndex(number) {#getColumnByIndex-number-}

Gets the [Column](../column/) object by the position in the list.

```javascript
getColumnByIndex(index: number) : Column;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The position in the list. |

**Returns**

Returns the column object.


