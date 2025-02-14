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
| [getSheetNames()](#getSheetNames--)| Names of all the worksheets this instance references to. |
| [isEntireRow()](#isEntireRow--)| Indicates whether this area contains all columns(entire row). |
| [isEntireColumn()](#isEntireColumn--)| Indicates whether this area contains all rows(entire column). |
| [isArea()](#isArea--)| Indicates whether this is an area. |
| [getEndColumn()](#getEndColumn--)| The end column of the area. |
| [getStartColumn()](#getStartColumn--)| The start column of the area. |
| [getEndRow()](#getEndRow--)| The end row of the area. |
| [getStartRow()](#getStartRow--)| The start row of the area. |
| [getValues()](#getValues--)| Gets cell values in this area. |
| [getValues(boolean)](#getValues-boolean-)| Gets cell values in this area. |
| [getValue(number, number)](#getValue-number-number-)| Gets cell value with given offset from the top-left of this area. |
| [getValue(number, number, boolean)](#getValue-number-number-boolean-)| Gets cell value with given offset from the top-left of this area. |
| [toString()](#toString--)| Returns the reference address of this area. Generally it is the address of the reference which may be used in formula, such as "Sheet1!A1:C3". |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


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


**Remarks**

If it references to multiple worksheets, the returned value is just like the range expression in the formula. For example "Sheet1:Sheet3" for the reference in formula "=SUM(Sheet1:Sheet3!$A$1:$B$2)".

### getSheetNames() {#getSheetNames--}

Names of all the worksheets this instance references to.

```javascript
getSheetNames() : string[];
```


**Returns**

string[]

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


### getValues() {#getValues--}

Gets cell values in this area.

```javascript
getValues() : object;
```


**Returns**

If this area is invalid, "#REF!" will be returned; If this area is one single cell, then return the cell value object; Otherwise return one 2D array for all values in this area.

### getValues(boolean) {#getValues-boolean-}

Gets cell values in this area.

```javascript
getValues(calculateFormulas: boolean) : object;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| calculateFormulas | boolean | In this range, if there are some formulas that have not been calculated,         /// this flag denotes whether those formulas should be calculated recursively |

**Returns**

If this area is invalid, "#REF!" will be returned; If this area is one single cell, then return the cell value object; Otherwise return one 2D array for all values in this area.

### getValue(number, number) {#getValue-number-number-}

Gets cell value with given offset from the top-left of this area.

```javascript
getValue(rowOffset: number, colOffset: number) : object;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | number | row offset from the start row of this area |
| colOffset | number | column offset from the start row of this area |

**Returns**

"#REF!" if this area is invalid; "#N/A" if given offset out of this area; Otherwise return the cell value at given position.

### getValue(number, number, boolean) {#getValue-number-number-boolean-}

Gets cell value with given offset from the top-left of this area.

```javascript
getValue(rowOffset: number, colOffset: number, calculateFormulas: boolean) : object;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | number | row offset from the start row of this area |
| colOffset | number | column offset from the start row of this area |
| calculateFormulas | boolean | Whether calculate it recursively if the specified reference is formula |

**Returns**

"#REF!" if this area is invalid; "#N/A" if given offset out of this area; Otherwise return the cell value at given position.

### toString() {#toString--}

Returns the reference address of this area. Generally it is the address of the reference which may be used in formula, such as "Sheet1!A1:C3".

```javascript
toString() : string;
```


**Returns**

the reference address of this area.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



