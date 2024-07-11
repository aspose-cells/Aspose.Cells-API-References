---
title: RevisionInsertSheet
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a revision record of a sheet that was inserted.
type: docs
url: /nodejs-cpp/revisioninsertsheet/
---

## RevisionInsertSheet class

Represents a revision record of a sheet that was inserted.

```javascript
class RevisionInsertSheet extends Revision;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the type of revision. |
| [getActionType()](#getActionType--)| Gets the action type of the revision. |
| [getName()](#getName--)| Gets the name of the worksheet. |
| [getSheetPosition()](#getSheetPosition--)| Gets the zero based position of the new sheet in the sheet tab bar. |
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

[RevisionType](./revisiontype/)

### getActionType() {#getActionType--}

Gets the action type of the revision.

```javascript
getActionType() : RevisionActionType;
```


**Returns**

[RevisionActionType](./revisionactiontype/)

### getName() {#getName--}

Gets the name of the worksheet.

```javascript
getName() : string;
```


### getSheetPosition() {#getSheetPosition--}

Gets the zero based position of the new sheet in the sheet tab bar.

```javascript
getSheetPosition() : number;
```


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


