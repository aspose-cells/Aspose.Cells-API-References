﻿---
title: Name
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a defined name for a range of cells.
type: docs
url: /nodejs-cpp/name/
---

## Name class

Represents a defined name for a range of cells.

```javascript
class Name;
```


## Methods

| Method | Description |
| --- | --- |
| [getComment()](#getComment--)| Gets and sets the comment of the name. Only applies for Excel 2007 or higher versions. |
| [setComment(string)](#setComment-string-)| Gets and sets the comment of the name. Only applies for Excel 2007 or higher versions. |
| [getText()](#getText--)| Gets the name text of the object. |
| [setText(string)](#setText-string-)| Gets the name text of the object. |
| [getFullText()](#getFullText--)| Gets the name  full text of the object with the scope setting. |
| [getR1C1RefersTo()](#getR1C1RefersTo--)| Gets or sets a R1C1 reference of the [Name](./name/). |
| [setR1C1RefersTo(string)](#setR1C1RefersTo-string-)| Gets or sets a R1C1 reference of the [Name](./name/). |
| [isReferred()](#isReferred--)| Indicates whether this name is referred by other formulas. |
| [isVisible()](#isVisible--)| Indicates whether the name is visible. |
| [setIsVisible(boolean)](#setIsVisible-boolean-)| Indicates whether the name is visible. |
| [getSheetIndex()](#getSheetIndex--)| Indicates this name belongs to Workbook or Worksheet. 0 = Global name, otherwise index to sheet (one-based) |
| [setSheetIndex(number)](#setSheetIndex-number-)| Indicates this name belongs to Workbook or Worksheet. 0 = Global name, otherwise index to sheet (one-based) |
| [getRefersTo(boolean, boolean)](#getRefersTo-boolean-boolean-)| Get the reference of this Name. |
| [getRefersTo(boolean, boolean, number, number)](#getRefersTo-boolean-boolean-number-number-)| Get the reference of this Name based on specified cell. |
| [setRefersTo(string, boolean, boolean)](#setRefersTo-string-boolean-boolean-)| Set the reference of this Name. |
| [toString()](#toString--)| Returns a string represents the current Range object. |
| [getRanges()](#getRanges--)| Gets all ranges referred by this name. |
| [getRanges(boolean)](#getRanges-boolean-)| Gets all ranges referred by this name. |
| [getReferredAreas(boolean)](#getReferredAreas-boolean-)| Gets all references referred by this name. |
| [getRange()](#getRange--)| Gets the range if this name refers to a range. |
| [getRange(boolean)](#getRange-boolean-)| Gets the range if this name refers to a range |
| [getRange(number, number, number)](#getRange-number-number-number-)| Gets the range if this name refers to a range. If the reference of this name is not absolute, the range may be different for different cell. |


### getComment() {#getComment--}

Gets and sets the comment of the name. Only applies for Excel 2007 or higher versions.

```javascript
getComment() : string;
```


### setComment(string) {#setComment-string-}

Gets and sets the comment of the name. Only applies for Excel 2007 or higher versions.

```javascript
setComment(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getText() {#getText--}

Gets the name text of the object.

```javascript
getText() : string;
```


### setText(string) {#setText-string-}

Gets the name text of the object.

```javascript
setText(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getFullText() {#getFullText--}

Gets the name  full text of the object with the scope setting.

```javascript
getFullText() : string;
```


### getR1C1RefersTo() {#getR1C1RefersTo--}

Gets or sets a R1C1 reference of the [Name](./name/).

```javascript
getR1C1RefersTo() : string;
```


### setR1C1RefersTo(string) {#setR1C1RefersTo-string-}

Gets or sets a R1C1 reference of the [Name](./name/).

```javascript
setR1C1RefersTo(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isReferred() {#isReferred--}

Indicates whether this name is referred by other formulas.

```javascript
isReferred() : boolean;
```


### isVisible() {#isVisible--}

Indicates whether the name is visible.

```javascript
isVisible() : boolean;
```


### setIsVisible(boolean) {#setIsVisible-boolean-}

Indicates whether the name is visible.

```javascript
setIsVisible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSheetIndex() {#getSheetIndex--}

Indicates this name belongs to Workbook or Worksheet. 0 = Global name, otherwise index to sheet (one-based)

```javascript
getSheetIndex() : number;
```


### setSheetIndex(number) {#setSheetIndex-number-}

Indicates this name belongs to Workbook or Worksheet. 0 = Global name, otherwise index to sheet (one-based)

```javascript
setSheetIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getRefersTo(boolean, boolean) {#getRefersTo-boolean-boolean-}

Get the reference of this Name.

```javascript
getRefersTo(isR1C1: boolean, isLocal: boolean) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the reference needs to be formatted as R1C1. |
| isLocal | boolean | Whether the reference needs to be formatted by locale. |

### getRefersTo(boolean, boolean, number, number) {#getRefersTo-boolean-boolean-number-number-}

Get the reference of this Name based on specified cell.

```javascript
getRefersTo(isR1C1: boolean, isLocal: boolean, row: number, column: number) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the reference needs to be formatted as R1C1. |
| isLocal | boolean | Whether the reference needs to be formatted by locale. |
| row | number | The row index of the cell. |
| column | number | The column index of the cell. |

### setRefersTo(string, boolean, boolean) {#setRefersTo-string-boolean-boolean-}

Set the reference of this Name.

```javascript
setRefersTo(refersTo: string, isR1C1: boolean, isLocal: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| refersTo | string | The reference. |
| isR1C1 | boolean | Whether the reference is R1C1 format. |
| isLocal | boolean | Whether the reference is locale formatted. |

### toString() {#toString--}

Returns a string represents the current Range object.

```javascript
toString() : string;
```


### getRanges() {#getRanges--}

Gets all ranges referred by this name.

```javascript
getRanges() : Range[];
```


**Returns**

All ranges.

### getRanges(boolean) {#getRanges-boolean-}

Gets all ranges referred by this name.

```javascript
getRanges(recalculate: boolean) : Range[];
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | boolean | whether recalculate it if this name has been calculated before this invocation. |

**Returns**

All ranges.

### getReferredAreas(boolean) {#getReferredAreas-boolean-}

Gets all references referred by this name.

```javascript
getReferredAreas(recalculate: boolean) : ReferredArea[];
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | boolean | whether recalculate it if this name has been calculated before this invocation. |

**Returns**

All ranges.

### getRange() {#getRange--}

Gets the range if this name refers to a range.

```javascript
getRange() : Range;
```


**Returns**

The range.

### getRange(boolean) {#getRange-boolean-}

Gets the range if this name refers to a range

```javascript
getRange(recalculate: boolean) : Range;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | boolean | whether recalculate it if this name has been calculated before this invocation. |

**Returns**

The range.

### getRange(number, number, number) {#getRange-number-number-number-}

Gets the range if this name refers to a range. If the reference of this name is not absolute, the range may be different for different cell.

```javascript
getRange(sheetIndex: number, row: number, column: number) : Range;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | number | The according sheet index. |
| row | number | The according row index. |
| column | number | The according column index |

**Returns**

The range.


