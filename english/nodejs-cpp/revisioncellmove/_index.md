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

| Constructor | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [type](#type--)| RevisionType | Readonly. Represents the type of revision. |
| [sourceArea](#sourceArea--)| CellArea | Readonly. Gets the source area. |
| [destinationArea](#destinationArea--)| CellArea | Readonly. Gets the destination area. |
| [sourceWorksheet](#sourceWorksheet--)| Worksheet | Readonly. Gets the source worksheet. |
| [worksheet](#worksheet--)| Worksheet | Readonly. Gets the worksheet. |
| [id](#id--)| number | Readonly. Gets the number of this revision. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Represents the type of revision. |
| [getSourceArea()](#getSourceArea--)| <b>@deprecated.</b> Please use the 'sourceArea' property instead. Gets the source area. |
| [getDestinationArea()](#getDestinationArea--)| <b>@deprecated.</b> Please use the 'destinationArea' property instead. Gets the destination area. |
| [getSourceWorksheet()](#getSourceWorksheet--)| <b>@deprecated.</b> Please use the 'sourceWorksheet' property instead. Gets the source worksheet. |
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

Readonly. Represents the type of revision.

```javascript
type : RevisionType;
```


### sourceArea {#sourceArea--}

Readonly. Gets the source area.

```javascript
sourceArea : CellArea;
```


### destinationArea {#destinationArea--}

Readonly. Gets the destination area.

```javascript
destinationArea : CellArea;
```


### sourceWorksheet {#sourceWorksheet--}

Readonly. Gets the source worksheet.

```javascript
sourceWorksheet : Worksheet;
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

<b>@deprecated.</b> Please use the 'type' property instead. Represents the type of revision.

```javascript
getType() : RevisionType;
```


**Returns**

[RevisionType](../revisiontype/)

### getSourceArea() {#getSourceArea--}

<b>@deprecated.</b> Please use the 'sourceArea' property instead. Gets the source area.

```javascript
getSourceArea() : CellArea;
```


**Returns**

[CellArea](../cellarea/)

### getDestinationArea() {#getDestinationArea--}

<b>@deprecated.</b> Please use the 'destinationArea' property instead. Gets the destination area.

```javascript
getDestinationArea() : CellArea;
```


**Returns**

[CellArea](../cellarea/)

### getSourceWorksheet() {#getSourceWorksheet--}

<b>@deprecated.</b> Please use the 'sourceWorksheet' property instead. Gets the source worksheet.

```javascript
getSourceWorksheet() : Worksheet;
```


**Returns**

[Worksheet](../worksheet/)

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


