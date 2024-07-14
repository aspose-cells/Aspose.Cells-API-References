---
title: RevisionAutoFormat
second_title: Aspose.Cells for Node.js via C++ API Reference
description: represents a revision record of information about a formatting change.
type: docs
url: /nodejs-cpp/revisionautoformat/
---

## RevisionAutoFormat class

represents a revision record of information about a formatting change.

```javascript
class RevisionAutoFormat extends Revision;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the type of the revision. |
| [getCellArea()](#getCellArea--)| Gets the location where the formatting was applied. |
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

Gets the type of the revision.

```javascript
getType() : RevisionType;
```


**Returns**

[RevisionType](/nodejs-cpp/revisiontype/)

### getCellArea() {#getCellArea--}

Gets the location where the formatting was applied.

```javascript
getCellArea() : CellArea;
```


**Returns**

[CellArea](/nodejs-cpp/cellarea/)

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


