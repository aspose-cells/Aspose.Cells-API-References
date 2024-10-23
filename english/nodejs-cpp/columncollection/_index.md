﻿---
title: ColumnCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Collection of the Column..column objects that represent the individual columnsettings in a worksheet. The Column object only represents the settings such as column width styles .etc. for the whole column has nothing to do with the fact that there are nonempty cellsdata or not in corresponding column. And the Count of this collection only represents the count Column objects that have been instantiated in this collection has nothing to do with the fact that there are nonempty cellsdata or not in the worksheet.
type: docs
url: /nodejs-cpp/columncollection/
---

## ColumnCollection class

Collection of the [Column](../column/) objects that represent the individual column(setting)s in a worksheet. The Column object only represents the settings such as column width, styles, .etc. for the whole column, has nothing to do with the fact that there are non-empty cells(data) or not in corresponding column. And the "Count" of this collection only represents the count Column objects that have been instantiated in this collection, has nothing to do with the fact that there are non-empty cells(data) or not in the worksheet.

```javascript
class ColumnCollection;
```


### Example
```javascript
const { Workbook, Color, BackgroundType, StyleFlag } = require("aspose.cells.node");

//Instantiating a Workbook object
var workbook = new Workbook();
//Obtaining the reference of the first worksheet
var worksheet = workbook.getWorksheets().get(0);
//Add new Style to Workbook
var style = workbook.createStyle();
//Setting the background color to Blue
style.setForegroundColor(new Color(0, 0, 0xff));
//setting Background Pattern
style.setPattern(BackgroundType.Solid);
//New Style Flag
var styleFlag = new StyleFlag();
//Set All Styles
styleFlag.setAll(true);

//Change the default width of first ten columns
for (var i = 0; i < 10; i++)
{
    worksheet.getCells().getColumns().get(i).setWidth(20);
}

//Get the Column with non default formatting
var columns = worksheet.getCells().getColumns();
var count = columns.getCount();
for (var i = 0; i < count; i++)
{
    var column = columns.getColumnByIndex(i);
    //Apply Style to first ten Columns
    column.applyStyle(style, styleFlag);
}

//Saving the Excel file
workbook.save("output/ColumnCollection.xls");
```
## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets a [Column](../column/) object by column index. The Column object of given column index will be instantiated if it does not exist before. |
| [getColumnByIndex(number)](#getColumnByIndex-number-)| Gets the [Column](../column/) object by the position in the list. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


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

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



