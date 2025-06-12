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

| Constructor | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [type](#type--)| RevisionType | Readonly. Gets the type of revision. |
| [row](#row--)| number | Readonly. Gets the row index of the which contains a comment. |
| [column](#column--)| number | Readonly. Gets the column index of the which contains a comment. |
| [cellName](#cellName--)| string | Gets the name of the cell. |
| [actionType](#actionType--)| RevisionActionType | Readonly. Gets the action type of the revision. |
| [isOldComment](#isOldComment--)| boolean | Readonly. Indicates whether it's an  old comment. |
| [oldLength](#oldLength--)| number | Readonly. Gets Length of the comment text added in this revision. |
| [newLength](#newLength--)| number | Readonly. Gets Length of the comment before this revision was made. |
| [worksheet](#worksheet--)| Worksheet | Readonly. Gets the worksheet. |
| [id](#id--)| number | Readonly. Gets the number of this revision. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets the type of revision. |
| [getRow()](#getRow--)| <b>@deprecated.</b> Please use the 'row' property instead. Gets the row index of the which contains a comment. |
| [getColumn()](#getColumn--)| <b>@deprecated.</b> Please use the 'column' property instead. Gets the column index of the which contains a comment. |
| [getCellName()](#getCellName--)| <b>@deprecated.</b> Please use the 'cellName' property instead. Gets the name of the cell. |
| [setCellName(string)](#setCellName-string-)| <b>@deprecated.</b> Please use the 'cellName' property instead. Gets the name of the cell. |
| [getActionType()](#getActionType--)| <b>@deprecated.</b> Please use the 'actionType' property instead. Gets the action type of the revision. |
| [isOldComment()](#isOldComment--)| <b>@deprecated.</b> Please use the 'isOldComment' property instead. Indicates whether it's an  old comment. |
| [getOldLength()](#getOldLength--)| <b>@deprecated.</b> Please use the 'oldLength' property instead. Gets Length of the comment text added in this revision. |
| [getNewLength()](#getNewLength--)| <b>@deprecated.</b> Please use the 'newLength' property instead. Gets Length of the comment before this revision was made. |
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

Readonly. Gets the type of revision.

```javascript
type : RevisionType;
```


### row {#row--}

Readonly. Gets the row index of the which contains a comment.

```javascript
row : number;
```


### column {#column--}

Readonly. Gets the column index of the which contains a comment.

```javascript
column : number;
```


### cellName {#cellName--}

Gets the name of the cell.

```javascript
cellName : string;
```


### actionType {#actionType--}

Readonly. Gets the action type of the revision.

```javascript
actionType : RevisionActionType;
```


### isOldComment {#isOldComment--}

Readonly. Indicates whether it's an  old comment.

```javascript
isOldComment : boolean;
```


### oldLength {#oldLength--}

Readonly. Gets Length of the comment text added in this revision.

```javascript
oldLength : number;
```


### newLength {#newLength--}

Readonly. Gets Length of the comment before this revision was made.

```javascript
newLength : number;
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

<b>@deprecated.</b> Please use the 'type' property instead. Gets the type of revision.

```javascript
getType() : RevisionType;
```


**Returns**

[RevisionType](../revisiontype/)

### getRow() {#getRow--}

<b>@deprecated.</b> Please use the 'row' property instead. Gets the row index of the which contains a comment.

```javascript
getRow() : number;
```


### getColumn() {#getColumn--}

<b>@deprecated.</b> Please use the 'column' property instead. Gets the column index of the which contains a comment.

```javascript
getColumn() : number;
```


### getCellName() {#getCellName--}

<b>@deprecated.</b> Please use the 'cellName' property instead. Gets the name of the cell.

```javascript
getCellName() : string;
```


### setCellName(string) {#setCellName-string-}

<b>@deprecated.</b> Please use the 'cellName' property instead. Gets the name of the cell.

```javascript
setCellName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getActionType() {#getActionType--}

<b>@deprecated.</b> Please use the 'actionType' property instead. Gets the action type of the revision.

```javascript
getActionType() : RevisionActionType;
```


**Returns**

[RevisionActionType](../revisionactiontype/)

### isOldComment() {#isOldComment--}

<b>@deprecated.</b> Please use the 'isOldComment' property instead. Indicates whether it's an  old comment.

```javascript
isOldComment() : boolean;
```


### getOldLength() {#getOldLength--}

<b>@deprecated.</b> Please use the 'oldLength' property instead. Gets Length of the comment text added in this revision.

```javascript
getOldLength() : number;
```


### getNewLength() {#getNewLength--}

<b>@deprecated.</b> Please use the 'newLength' property instead. Gets Length of the comment before this revision was made.

```javascript
getNewLength() : number;
```


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


