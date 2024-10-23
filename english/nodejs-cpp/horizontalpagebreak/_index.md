---
title: HorizontalPageBreak
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents a horizontal page break.
type: docs
url: /nodejs-cpp/horizontalpagebreak/
---

## HorizontalPageBreak class

Encapsulates the object that represents a horizontal page break.

```javascript
class HorizontalPageBreak;
```


### Example
```javascript
const { Workbook } = require("aspose.cells.node");

//Instantiating a Workbook object
var workbook = new Workbook();

//Obtaining the reference of the newly added worksheet by passing its sheet index
var worksheet = workbook.getWorksheets().get(0);

//Add a page break at cell Y30
var Index = worksheet.getHorizontalPageBreaks().add("Y30");

//get the newly added horizontal page break
var hPageBreak = worksheet.getHorizontalPageBreaks().get(Index);
```
## Methods

| Method | Description |
| --- | --- |
| [getStartColumn()](#getStartColumn--)| Gets the start column index of this horizontal page break. |
| [getEndColumn()](#getEndColumn--)| Gets the end column index of this horizontal page break. |
| [getRow()](#getRow--)| Gets the zero based row index. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getStartColumn() {#getStartColumn--}

Gets the start column index of this horizontal page break.

```javascript
getStartColumn() : number;
```


### getEndColumn() {#getEndColumn--}

Gets the end column index of this horizontal page break.

```javascript
getEndColumn() : number;
```


### getRow() {#getRow--}

Gets the zero based row index.

```javascript
getRow() : number;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



