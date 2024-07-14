---
title: RevisionFormat
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a revision record of information about a formatting change.
type: docs
url: /nodejs-cpp/revisionformat/
---

## RevisionFormat class

Represents a revision record of information about a formatting change.

```javascript
class RevisionFormat extends Revision;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the type of revision. |
| [getAreas()](#getAreas--)| The range to which this formatting was applied. |
| [getStyle()](#getStyle--)| Gets the applied style. |
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

### getAreas() {#getAreas--}

The range to which this formatting was applied.

```javascript
getAreas() : CellArea[];
```


**Returns**

[CellArea](/nodejs-cpp/cellarea/)[]

### getStyle() {#getStyle--}

Gets the applied style.

```javascript
getStyle() : Style;
```


**Returns**

[Style](/nodejs-cpp/style/)

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


