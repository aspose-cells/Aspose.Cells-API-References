---
title: Revision
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the revision.
type: docs
url: /nodejs-cpp/revision/
---

## Revision class

Represents the revision.

```javascript
class Revision;
```


## Methods

| Method | Description |
| --- | --- |
| [getWorksheet()](#getWorksheet--)| Gets the worksheet. |
| [getId()](#getId--)| Gets the number of this revision. |
| [getType()](#getType--)| Represents the type of revision. |


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

### getType() {#getType--}

Represents the type of revision.

```javascript
getType() : RevisionType;
```


**Returns**

[RevisionType](/nodejs-cpp/revisiontype/)


