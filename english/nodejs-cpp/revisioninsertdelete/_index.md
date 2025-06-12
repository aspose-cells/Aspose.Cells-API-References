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

| Constructor | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [type](#type--)| RevisionType | Readonly. Represents the type of revision. |
| [cellArea](#cellArea--)| CellArea | Readonly. Gets the inserting/deleting range. |
| [actionType](#actionType--)| RevisionActionType | Readonly. Gets the action type of this revision. |
| [revisions](#revisions--)| RevisionCollection | Readonly. Gets revision list by this operation. |
| [worksheet](#worksheet--)| Worksheet | Readonly. Gets the worksheet. |
| [id](#id--)| number | Readonly. Gets the number of this revision. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Represents the type of revision. |
| [getCellArea()](#getCellArea--)| <b>@deprecated.</b> Please use the 'cellArea' property instead. Gets the inserting/deleting range. |
| [getActionType()](#getActionType--)| <b>@deprecated.</b> Please use the 'actionType' property instead. Gets the action type of this revision. |
| [getRevisions()](#getRevisions--)| <b>@deprecated.</b> Please use the 'revisions' property instead. Gets revision list by this operation. |
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


### cellArea {#cellArea--}

Readonly. Gets the inserting/deleting range.

```javascript
cellArea : CellArea;
```


### actionType {#actionType--}

Readonly. Gets the action type of this revision.

```javascript
actionType : RevisionActionType;
```


### revisions {#revisions--}

Readonly. Gets revision list by this operation.

```javascript
revisions : RevisionCollection;
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

### getCellArea() {#getCellArea--}

<b>@deprecated.</b> Please use the 'cellArea' property instead. Gets the inserting/deleting range.

```javascript
getCellArea() : CellArea;
```


**Returns**

[CellArea](../cellarea/)

### getActionType() {#getActionType--}

<b>@deprecated.</b> Please use the 'actionType' property instead. Gets the action type of this revision.

```javascript
getActionType() : RevisionActionType;
```


**Returns**

[RevisionActionType](../revisionactiontype/)

### getRevisions() {#getRevisions--}

<b>@deprecated.</b> Please use the 'revisions' property instead. Gets revision list by this operation.

```javascript
getRevisions() : RevisionCollection;
```


**Returns**

[RevisionCollection](../revisioncollection/)

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


