---
title: RevisionCellMove
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a revision record on a cells that moved.
type: docs
url: /nodejs-cpp/revisioncellmove/
---

## RevisionCellMove class

Represents a revision record on a cell(s) that moved.

```javascript
class RevisionCellMove extends Revision;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Represents the type of revision. |
| [getSourceArea()](#getSourceArea--)| Gets the source area. |
| [getDestinationArea()](#getDestinationArea--)| Gets the destination area. |
| [getSourceWorksheet()](#getSourceWorksheet--)| Gets the source worksheet. |
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

### getSourceArea() {#getSourceArea--}

Gets the source area.

```javascript
getSourceArea() : CellArea;
```


**Returns**

[CellArea](../cellarea/)

### getDestinationArea() {#getDestinationArea--}

Gets the destination area.

```javascript
getDestinationArea() : CellArea;
```


**Returns**

[CellArea](../cellarea/)

### getSourceWorksheet() {#getSourceWorksheet--}

Gets the source worksheet.

```javascript
getSourceWorksheet() : Worksheet;
```


**Returns**

[Worksheet](../worksheet/)

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


