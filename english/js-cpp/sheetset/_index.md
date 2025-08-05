﻿---
title: SheetSet
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Describes a set of sheets.
type: docs
url: /js-cpp/sheetset/
---

## SheetSet class

Describes a set of sheets.

```javascript
class SheetSet;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(number[])](#constructor-numberarray-)| Creates a sheet set based on exact sheet indexes. |
| [constructor(string[])](#constructor-stringarray-)| Creates a sheet set based on exact sheet names. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| static [active](#active--)| SheetSet | Readonly. Gets a set with active sheet of the workbook. |
| static [visible](#visible--)| SheetSet | Readonly. Gets a set with visible sheets of the workbook in their original order. |
| static [all](#all--)| SheetSet | Readonly. Gets a set with all sheets of the workbook in their original order. |


### constructor(number[]) {#constructor-numberarray-}

Creates a sheet set based on exact sheet indexes.

```javascript
constructor(sheetIndexes: number[]);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndexes | number[] | zero based sheet indexes. |

**Remarks**

If a sheet is encountered that is not in the workbook, an exception will be thrown during rendering.

### constructor(string[]) {#constructor-stringarray-}

Creates a sheet set based on exact sheet names.

```javascript
constructor(sheetNames: string[]);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetNames | string[] | sheet names. |

**Remarks**

If a sheet is encountered that is not in the workbook, an exception will be thrown during rendering.

### active {#active--}

Readonly. Gets a set with active sheet of the workbook.

```javascript
static active : SheetSet;
```


### visible {#visible--}

Readonly. Gets a set with visible sheets of the workbook in their original order.

```javascript
static visible : SheetSet;
```


### all {#all--}

Readonly. Gets a set with all sheets of the workbook in their original order.

```javascript
static all : SheetSet;
```



