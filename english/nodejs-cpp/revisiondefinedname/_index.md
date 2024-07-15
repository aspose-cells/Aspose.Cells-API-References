---
title: RevisionDefinedName
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a revision record of a defined name change.
type: docs
url: /nodejs-cpp/revisiondefinedname/
---

## RevisionDefinedName class

Represents a revision record of a defined name change.

```javascript
class RevisionDefinedName extends Revision;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(Revision)](#constructor-revision-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Represents the type of revision. |
| [getText()](#getText--)| Gets the text of the defined name. |
| [getOldFormula()](#getOldFormula--)| Gets the old formula. |
| [getNewFormula()](#getNewFormula--)| Gets the formula. |
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

Represents the type of revision.

```javascript
getType() : RevisionType;
```


**Returns**

[RevisionType](../revisiontype/)

### getText() {#getText--}

Gets the text of the defined name.

```javascript
getText() : string;
```


### getOldFormula() {#getOldFormula--}

Gets the old formula.

```javascript
getOldFormula() : string;
```


### getNewFormula() {#getNewFormula--}

Gets the formula.

```javascript
getNewFormula() : string;
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


