---
title: TableStyle
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the style of the table.
type: docs
url: /nodejs-cpp/tablestyle/
---

## TableStyle class

Represents the style of the table.

```javascript
class TableStyle;
```


### Example
```javascript
const { Workbook, BackgroundType, Color, TableStyleElementType, CellsHelper } = require("aspose.cells.node");

var workbook = new Workbook();
var firstColumnStyle = workbook.createStyle();
firstColumnStyle.pattern = BackgroundType.Solid;
firstColumnStyle.backgroundColor = Color.Red;

var lastColumnStyle = workbook.createStyle();
lastColumnStyle.font.isBold = true;
lastColumnStyle.pattern = BackgroundType.Solid;
lastColumnStyle.backgroundColor = Color.Red;
var tableStyleName = "Custom1";
var tableStyles = workbook.worksheets.getTableStyles();
var index1 = tableStyles.addTableStyle(tableStyleName);
var tableStyle = tableStyles.get(index1);
var elements = tableStyle.getTableStyleElements();
index1 = elements.add(TableStyleElementType.FirstColumn);
var element = elements.get(index1);
element.setElementStyle(firstColumnStyle);
index1 = elements.add(TableStyleElementType.LastColumn);
element = elements.get(index1);
element.setElementStyle(lastColumnStyle);
var cells = workbook.worksheets.get(0).cells;
for (var i = 0; i < 5; i++) {
    cells.get(0, i).putValue(CellsHelper.columnIndexToName(i));
}
for (var row = 1; row < 10; row++) {
    for (var column = 0; column < 5; column++) {
        cells.get(row, column).putValue(row * column);
    }
}
var tables = workbook.worksheets.get(0).getListObjects();
var index = tables.add(0, 0, 9, 4, true);
var table = tables.get(0);
table.showTableStyleFirstColumn = true;
table.showTableStyleLastColumn = true;
table.tableStyleName = tableStyleName;
workbook.save("output/TablesTableStyle.xlsx");
```
## Properties

| Property | Type | Description |
| --- | --- | --- |
| [name](#name--)| string | Readonly. Gets the name of table style. |
| [tableStyleElements](#tableStyleElements--)| TableStyleElementCollection | Readonly. Gets all elements of the table style. |

## Methods

| Method | Description |
| --- | --- |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets the name of table style. |
| [getTableStyleElements()](#getTableStyleElements--)| <b>@deprecated.</b> Please use the 'tableStyleElements' property instead. Gets all elements of the table style. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### name {#name--}

Readonly. Gets the name of table style.

```javascript
name : string;
```


### tableStyleElements {#tableStyleElements--}

Readonly. Gets all elements of the table style.

```javascript
tableStyleElements : TableStyleElementCollection;
```


### getName() {#getName--}

<b>@deprecated.</b> Please use the 'name' property instead. Gets the name of table style.

```javascript
getName() : string;
```


### getTableStyleElements() {#getTableStyleElements--}

<b>@deprecated.</b> Please use the 'tableStyleElements' property instead. Gets all elements of the table style.

```javascript
getTableStyleElements() : TableStyleElementCollection;
```


**Returns**

[TableStyleElementCollection](../tablestyleelementcollection/)

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



