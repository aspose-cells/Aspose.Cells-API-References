---
title: RevisionCellChange
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the revision that changing cells.
type: docs
url: /nodejs-cpp/revisioncellchange/
---

## RevisionCellChange class

Represents the revision that changing cells.

```javascript
class RevisionCellChange extends Revision;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Represents the type of revision. |
| [getCellName()](#getCellName--)| Gets the name of the cell. |
| [getRow()](#getRow--)| Gets the row index of the cell. |
| [getColumn()](#getColumn--)| Gets the column index of the cell. |
| [isNewFormatted()](#isNewFormatted--)| Indicates whether this cell is new formatted. |
| [isOldFormatted()](#isOldFormatted--)| Indicates whether this cell is old formatted. |
| [getOldFormula()](#getOldFormula--)| Gets the old formula. |
| [getNewFormula()](#getNewFormula--)| Gets the old formula. |
| [getNewStyle()](#getNewStyle--)| Gets the new style of the cell. |
| [getOldStyle()](#getOldStyle--)| Gets the old style of the cell. |
| [getWorksheet()](#getWorksheet--)| Gets the worksheet. |
| [getId()](#getId--)| Gets the number of this revision. |


### constructor(Revision) {#constructor-revision-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: Revision);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Revision | The parent object. |

### getType() {#getType--}

Represents the type of revision.

```javascript
getType() : RevisionType;
```


**Returns**

[RevisionType](../revisiontype/)

### getCellName() {#getCellName--}

Gets the name of the cell.

```javascript
getCellName() : string;
```


### getRow() {#getRow--}

Gets the row index of the cell.

```javascript
getRow() : number;
```


### getColumn() {#getColumn--}

Gets the column index of the cell.

```javascript
getColumn() : number;
```


### isNewFormatted() {#isNewFormatted--}

Indicates whether this cell is new formatted.

```javascript
isNewFormatted() : boolean;
```


### isOldFormatted() {#isOldFormatted--}

Indicates whether this cell is old formatted.

```javascript
isOldFormatted() : boolean;
```


### getOldFormula() {#getOldFormula--}

Gets the old formula.

```javascript
getOldFormula() : string;
```


### getNewFormula() {#getNewFormula--}

Gets the old formula.

```javascript
getNewFormula() : string;
```


### getNewStyle() {#getNewStyle--}

Gets the new style of the cell.

```javascript
getNewStyle() : Style;
```


**Returns**

[Style](../style/)

### getOldStyle() {#getOldStyle--}

Gets the old style of the cell.

```javascript
getOldStyle() : Style;
```


**Returns**

[Style](../style/)

### getWorksheet() {#getWorksheet--}

Gets the worksheet.

```javascript
getWorksheet() : Worksheet;
```


**Returns**

[Worksheet](../worksheet/)

### getId() {#getId--}

Gets the number of this revision.

```javascript
getId() : number;
```


**Remarks**

Zero means this revision does not contains id.


