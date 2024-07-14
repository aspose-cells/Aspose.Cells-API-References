---
title: RevisionCellComment
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a revision record of a cell comment change.
type: docs
url: /nodejs-cpp/revisioncellcomment/
---

## RevisionCellComment class

Represents a revision record of a cell comment change.

```javascript
class RevisionCellComment extends Revision;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the type of revision. |
| [getRow()](#getRow--)| Gets the row index of the which contains a comment. |
| [getColumn()](#getColumn--)| Gets the column index of the which contains a comment. |
| [getCellName()](#getCellName--)| Gets the name of the cell. |
| [setCellName(string)](#setCellName-string-)| Gets the name of the cell. |
| [getActionType()](#getActionType--)| Gets the action type of the revision. |
| [isOldComment()](#isOldComment--)| Indicates whether it's an  old comment. |
| [getOldLength()](#getOldLength--)| Gets Length of the comment text added in this revision. |
| [getNewLength()](#getNewLength--)| Gets Length of the comment before this revision was made. |
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

Gets the type of revision.

```javascript
getType() : RevisionType;
```


**Returns**

[RevisionType](/nodejs-cpp/revisiontype/)

### getRow() {#getRow--}

Gets the row index of the which contains a comment.

```javascript
getRow() : number;
```


### getColumn() {#getColumn--}

Gets the column index of the which contains a comment.

```javascript
getColumn() : number;
```


### getCellName() {#getCellName--}

Gets the name of the cell.

```javascript
getCellName() : string;
```


### setCellName(string) {#setCellName-string-}

Gets the name of the cell.

```javascript
setCellName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getActionType() {#getActionType--}

Gets the action type of the revision.

```javascript
getActionType() : RevisionActionType;
```


**Returns**

[RevisionActionType](/nodejs-cpp/revisionactiontype/)

### isOldComment() {#isOldComment--}

Indicates whether it's an  old comment.

```javascript
isOldComment() : boolean;
```


### getOldLength() {#getOldLength--}

Gets Length of the comment text added in this revision.

```javascript
getOldLength() : number;
```


### getNewLength() {#getNewLength--}

Gets Length of the comment before this revision was made.

```javascript
getNewLength() : number;
```


### getWorksheet() {#getWorksheet--}

Gets the worksheet.

```javascript
getWorksheet() : Worksheet;
```


**Returns**

[Worksheet](/nodejs-cpp/worksheet/)

### getId() {#getId--}

Gets the number of this revision.

```javascript
getId() : number;
```


**Remarks**

Zero means this revision does not contains id.


