---
title: VerticalPageBreak
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents a vertical page break.
type: docs
url: /nodejs-cpp/verticalpagebreak/
---

## VerticalPageBreak class

Encapsulates the object that represents a vertical page break.

```javascript
class VerticalPageBreak;
```


### Example
```javascript
const { Workbook } = require("aspose.cells.node");

var excel = new Workbook();
//Add a pagebreak at G5
excel.getWorksheets().get(0).getHorizontalPageBreaks().add("G5");
excel.getWorksheets().get(0).getVerticalPageBreaks().add("G5");
```
## Methods

| Method | Description |
| --- | --- |
| [getStartRow()](#getStartRow--)| Gets the start row index of the vertical page break. |
| [getEndRow()](#getEndRow--)| Gets the end row index of the vertical page break. |
| [getColumn()](#getColumn--)| Gets the column index of the vertical page break. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getStartRow() {#getStartRow--}

Gets the start row index of the vertical page break.

```javascript
getStartRow() : number;
```


### getEndRow() {#getEndRow--}

Gets the end row index of the vertical page break.

```javascript
getEndRow() : number;
```


### getColumn() {#getColumn--}

Gets the column index of the vertical page break.

```javascript
getColumn() : number;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



