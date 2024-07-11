---
title: ReferredArea
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a referred area by the formula.
type: docs
url: /nodejs-cpp/referredarea/
---

## ReferredArea class

Represents a referred area by the formula.

```javascript
class ReferredArea;
```


## Methods

| Method | Description |
| --- | --- |
| [isExternalLink()](#isExternalLink--)| Indicates whether this is an external link. |
| [getExternalFileName()](#getExternalFileName--)| Get the external file name if this is an external reference. |
| [getSheetName()](#getSheetName--)| Indicates which sheet this reference is in. |
| [isEntireRow()](#isEntireRow--)| Indicates whether this area contains all columns(entire row). |
| [isEntireColumn()](#isEntireColumn--)| Indicates whether this area contains all rows(entire column). |
| [isArea()](#isArea--)| Indicates whether this is an area. |
| [getEndColumn()](#getEndColumn--)| The end column of the area. |
| [getStartColumn()](#getStartColumn--)| The start column of the area. |
| [getEndRow()](#getEndRow--)| The end row of the area. |
| [getStartRow()](#getStartRow--)| The start row of the area. |
| [toString()](#toString--)| Returns the reference address of this area. Generally it is the address of the reference which may be used in formula, such as "Sheet1!A1:C3". |


### isExternalLink() {#isExternalLink--}

Indicates whether this is an external link.

```javascript
isExternalLink() : boolean;
```


### getExternalFileName() {#getExternalFileName--}

Get the external file name if this is an external reference.

```javascript
getExternalFileName() : string;
```


### getSheetName() {#getSheetName--}

Indicates which sheet this reference is in.

```javascript
getSheetName() : string;
```


### isEntireRow() {#isEntireRow--}

Indicates whether this area contains all columns(entire row).

```javascript
isEntireRow() : boolean;
```


### isEntireColumn() {#isEntireColumn--}

Indicates whether this area contains all rows(entire column).

```javascript
isEntireColumn() : boolean;
```


### isArea() {#isArea--}

Indicates whether this is an area.

```javascript
isArea() : boolean;
```


**Remarks**

If this is not an area, only StartRow and StartColumn effect.

### getEndColumn() {#getEndColumn--}

The end column of the area.

```javascript
getEndColumn() : number;
```


### getStartColumn() {#getStartColumn--}

The start column of the area.

```javascript
getStartColumn() : number;
```


### getEndRow() {#getEndRow--}

The end row of the area.

```javascript
getEndRow() : number;
```


### getStartRow() {#getStartRow--}

The start row of the area.

```javascript
getStartRow() : number;
```


### toString() {#toString--}

Returns the reference address of this area. Generally it is the address of the reference which may be used in formula, such as "Sheet1!A1:C3".

```javascript
toString() : string;
```


**Returns**

the reference address of this area.


