---
title: RevisionQueryTable
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a revision of a query table field change.
type: docs
url: /nodejs-cpp/revisionquerytable/
---

## RevisionQueryTable class

Represents a revision of a query table field change.

```javascript
class RevisionQueryTable extends Revision;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Represents the type of the revision. |
| [getCellArea()](#getCellArea--)| Gets the location of the affected query table. |
| [getFieldId()](#getFieldId--)| Gets ID of the specific query table field that was removed. |
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

Represents the type of the revision.

```javascript
getType() : RevisionType;
```


**Returns**

[RevisionType](../revisiontype/)

### getCellArea() {#getCellArea--}

Gets the location of the affected query table.

```javascript
getCellArea() : CellArea;
```


**Returns**

[CellArea](../cellarea/)

### getFieldId() {#getFieldId--}

Gets ID of the specific query table field that was removed.

```javascript
getFieldId() : number;
```


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


