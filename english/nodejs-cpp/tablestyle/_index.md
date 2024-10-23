---
title: TableStyle
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the table style.
type: docs
url: /nodejs-cpp/tablestyle/
---

## TableStyle class

Represents the table style.

```javascript
class TableStyle;
```


### Example
```javascript
const { Workbook, BackgroundType, Color, TableStyleElementType, CellsHelper } = require("aspose.cells.node");

var workbook = new Workbook();
var firstColumnStyle = workbook.createStyle();
firstColumnStyle.setPattern(BackgroundType.Solid);
firstColumnStyle.setBackgroundColor(new Color(0xff, 0, 0));

var lastColumnStyle = workbook.createStyle();
lastColumnStyle.getFont().setIsBold(true);
lastColumnStyle.setPattern(BackgroundType.Solid);
lastColumnStyle.setBackgroundColor(new Color(0xff, 0, 0));
var tableStyleName = "Custom1";
var tableStyles = workbook.getWorksheets().getTableStyles();
var index1 = tableStyles.addTableStyle(tableStyleName);
var tableStyle = tableStyles.get(index1);
var elements = tableStyle.getTableStyleElements();
index1 = elements.add(TableStyleElementType.FirstColumn);
var element = elements.get(index1);
element.setElementStyle(firstColumnStyle);
index1 = elements.add(TableStyleElementType.LastColumn);
element = elements.get(index1);
element.setElementStyle(lastColumnStyle);
var cells = workbook.getWorksheets().get(0).getCells();
for (var i = 0; i < 5; i++)
{
    cells.get(0, i).putValue(CellsHelper.columnIndexToName(i));
}
for (var row = 1; row < 10; row++)
{
    for (var column = 0; column < 5; column++)
    {
        cells.get(row, column).putValue(row * column);
    }
}
var tables = workbook.getWorksheets().get(0).getListObjects();
var index = tables.add(0, 0, 9, 4, true);
var table = tables.get(0);
table.setShowTableStyleFirstColumn(true);
table.setShowTableStyleLastColumn(true);
table.setTableStyleName(tableStyleName);
workbook.save("output/TablesTableStyle.xlsx");
```
## Methods

| Method | Description |
| --- | --- |
| [getName()](#getName--)| Gets the name of table style. |
| [getTableStyleElements()](#getTableStyleElements--)| Gets all elements of the table style. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getName() {#getName--}

Gets the name of table style.

```javascript
getName() : string;
```


### getTableStyleElements() {#getTableStyleElements--}

Gets all elements of the table style.

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



