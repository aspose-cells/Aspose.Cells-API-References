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

| Constructor | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [type](#type--)| RevisionType | Readonly. Gets the type of the revision. |
| [cellArea](#cellArea--)| CellArea | Readonly. Gets the location where the formatting was applied. |
| [worksheet](#worksheet--)| Worksheet | Readonly. Gets the worksheet. |
| [id](#id--)| number | Readonly. Gets the number of this revision. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets the type of the revision. |
| [getCellArea()](#getCellArea--)| <b>@deprecated.</b> Please use the 'cellArea' property instead. Gets the location where the formatting was applied. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getWorksheet()](#getWorksheet--)| <b>@deprecated.</b> Please use the 'worksheet' property instead. Gets the worksheet. |
| [getId()](#getId--)| <b>@deprecated.</b> Please use the 'id' property instead. Gets the number of this revision. |


### constructor(Revision) {#constructor-revision-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: Revision);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Revision | The parent object. |

### type {#type--}

Readonly. Gets the type of the revision.

```javascript
type : RevisionType;
```


### cellArea {#cellArea--}

Readonly. Gets the location where the formatting was applied.

```javascript
cellArea : CellArea;
```


### worksheet {#worksheet--}

Readonly. Gets the worksheet.

```javascript
worksheet : Worksheet;
```


### id {#id--}

Readonly. Gets the number of this revision.

```javascript
id : number;
```


**Remarks**

Zero means this revision does not contains id.

### getType() {#getType--}

<b>@deprecated.</b> Please use the 'type' property instead. Gets the type of the revision.

```javascript
getType() : RevisionType;
```


**Returns**

[RevisionType](../revisiontype/)

### getCellArea() {#getCellArea--}

<b>@deprecated.</b> Please use the 'cellArea' property instead. Gets the location where the formatting was applied.

```javascript
getCellArea() : CellArea;
```


**Returns**

[CellArea](../cellarea/)

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getWorksheet() {#getWorksheet--}

<b>@deprecated.</b> Please use the 'worksheet' property instead. Gets the worksheet.

```javascript
getWorksheet() : Worksheet;
```


**Returns**

[Worksheet](../worksheet/)

### getId() {#getId--}

<b>@deprecated.</b> Please use the 'id' property instead. Gets the number of this revision.

```javascript
getId() : number;
```


**Remarks**

Zero means this revision does not contains id.


