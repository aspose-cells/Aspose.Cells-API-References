---
title: RevisionRenameSheet
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a revision of renaming sheet.
type: docs
url: /nodejs-cpp/revisionrenamesheet/
---

## RevisionRenameSheet class

Represents a revision of renaming sheet.

```javascript
class RevisionRenameSheet extends Revision;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Represents the type of the revision. |
| [getOldName()](#getOldName--)| Gets the old name of the worksheet. |
| [getNewName()](#getNewName--)| Gets the new name of the worksheet. |
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

### getOldName() {#getOldName--}

Gets the old name of the worksheet.

```javascript
getOldName() : string;
```


### getNewName() {#getNewName--}

Gets the new name of the worksheet.

```javascript
getNewName() : string;
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


