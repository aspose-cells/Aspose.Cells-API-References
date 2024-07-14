---
title: RevisionInsertDelete
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a revision record of a rowcolumn insertdelete action.
type: docs
url: /nodejs-cpp/revisioninsertdelete/
---

## RevisionInsertDelete class

Represents a revision record of a row/column insert/delete action.

```javascript
class RevisionInsertDelete extends Revision;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Represents the type of revision. |
| [getCellArea()](#getCellArea--)| Gets the inserting/deleting range. |
| [getActionType()](#getActionType--)| Gets the action type of this revision. |
| [getRevisions()](#getRevisions--)| Gets revision list by this operation. |
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

[RevisionType](./revisiontype/)

### getCellArea() {#getCellArea--}

Gets the inserting/deleting range.

```javascript
getCellArea() : CellArea;
```


**Returns**

[CellArea](./cellarea/)

### getActionType() {#getActionType--}

Gets the action type of this revision.

```javascript
getActionType() : RevisionActionType;
```


**Returns**

[RevisionActionType](./revisionactiontype/)

### getRevisions() {#getRevisions--}

Gets revision list by this operation.

```javascript
getRevisions() : RevisionCollection;
```


**Returns**

[RevisionCollection](./revisioncollection/)

### getWorksheet() {#getWorksheet--}

Gets the worksheet.

```javascript
getWorksheet() : Worksheet;
```


**Returns**

[Worksheet](./worksheet/)

### getId() {#getId--}

Gets the number of this revision.

```javascript
getId() : number;
```


**Remarks**

Zero means this revision does not contains id.


