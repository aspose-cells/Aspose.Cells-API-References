﻿---
title: RevisionCustomView
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a revision record of adding or removing a custom view to the workbook
type: docs
url: /nodejs-cpp/revisioncustomview/
---

## RevisionCustomView class

Represents a revision record of adding or removing a custom view to the workbook

```javascript
class RevisionCustomView extends Revision;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the type of revision. |
| [getActionType()](#getActionType--)| Gets the type of action. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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

[RevisionType](../revisiontype/)

### getActionType() {#getActionType--}

Gets the type of action.

```javascript
getActionType() : RevisionActionType;
```


**Returns**

[RevisionActionType](../revisionactiontype/)

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
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


