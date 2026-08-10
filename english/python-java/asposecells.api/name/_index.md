---
title: "Name Class"
linktitle: "Name"
articleTitle: "Name"
second_title: "Aspose.Cells for Python via Java"
description: "Represents a defined name for a range of cells."
type: docs
weight: 3840
url: /python-java/asposecells.api/name/
---

## Name class

Represents a defined name for a range of cells.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Comment](#comment) | String | Gets and sets the comment of the name. Only applies for Excel 2007 or higher versions. |
| [Text](#text) | String | Gets the name text of the object. |
| [FullText](#fulltext) | String | Gets the name full text of the object with the scope setting. |
| [RefersTo](#refersto) | String | Returns or sets the formula that the name is defined to refer to, beginning with an equal sign. |
| [R1C1RefersTo](#r1c1refersto) | String | Gets or sets a R1C1 reference of the Name . |
| [IsReferred](#isreferred) | boolean | Indicates whether this name is referred by other formulas. |
| [IsVisible](#isvisible) | boolean | Indicates whether the name is visible. |
| [SheetIndex](#sheetindex) | int | Indicates this name belongs to Workbook or Worksheet. 0 = Global name, otherwise index to sheet (one-based) |

## Methods

| Name | Description |
| --- | --- |
| [getRefersTo](#getrefersto) | Get the reference of this Name. |
| [setRefersTo](#setrefersto) | Set the reference of this Name. |
| [toString](#tostring) | Returns a string represents the current Range object. |
| [getRanges](#getranges) | Gets all ranges referred by this name. |
| [getReferredAreas](#getreferredareas) | Gets all references referred by this name. |
| [getRange](#getrange) | Gets the range if this name refers to a range. |

### Name.Comment property {#comment}

Gets and sets the comment of the name. Only applies for Excel 2007 or higher versions.

**Type:** String

### Name.Text property {#text}

Gets the name text of the object.

**Type:** String

### Name.FullText property {#fulltext}

Gets the name full text of the object with the scope setting.

**Type:** String

### Name.RefersTo property {#refersto}

Returns or sets the formula that the name is defined to refer to, beginning with an equal sign.

**Type:** String

### Name.R1C1RefersTo property {#r1c1refersto}

Gets or sets a R1C1 reference of the Name .

**Type:** String

### Name.IsReferred property {#isreferred}

Indicates whether this name is referred by other formulas.

**Type:** boolean

### Name.IsVisible property {#isvisible}

Indicates whether the name is visible.

**Type:** boolean

### Name.SheetIndex property {#sheetindex}

Indicates this name belongs to Workbook or Worksheet. 0 = Global name, otherwise index to sheet (one-based)

**Type:** int

### getRefersTo(isR1C1, isLocal) (1 of 2) {#getrefersto}

Get the reference of this Name.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the reference needs to be formatted as R1C1. |
| isLocal | boolean | Whether the reference needs to be formatted by locale. |

---

### getRefersTo(isR1C1, isLocal, row, column) (2 of 2) {#getrefersto-1}

Get the reference of this Name based on specified cell.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the reference needs to be formatted as R1C1. |
| isLocal | boolean | Whether the reference needs to be formatted by locale. |
| row | int | The row index of the cell. |
| column | int | The column index of the cell. |

### setRefersTo(refersTo, isR1C1, isLocal) {#setrefersto}

Set the reference of this Name.

| Parameter | Type | Description |
| --- | --- | --- |
| refersTo | String | The reference. |
| isR1C1 | boolean | Whether the reference is R1C1 format. |
| isLocal | boolean | Whether the reference is locale formatted. |

### toString() {#tostring}

Returns a string represents the current Range object.

### getRanges() (1 of 2) {#getranges}

Gets all ranges referred by this name.

**Returns:** All ranges.

---

### getRanges(recalculate) (2 of 2) {#getranges-1}

Gets all ranges referred by this name.

| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | boolean | whether recalculate it if this name has been calculated before this invocation. |

**Returns:** All ranges.

### getReferredAreas(recalculate) {#getreferredareas}

Gets all references referred by this name.

| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | boolean | whether recalculate it if this name has been calculated before this invocation. |

**Returns:** All ranges.

### getRange() (1 of 3) {#getrange}

Gets the range if this name refers to a range.

**Returns:** The range.

---

### getRange(recalculate) (2 of 3) {#getrange-1}

Gets the range if this name refers to a range

| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | boolean | whether recalculate it if this name has been calculated before this invocation. |

**Returns:** The range.

---

### getRange(sheetIndex, row, column) (3 of 3) {#getrange-2}

Gets the range if this name refers to a range. If the reference of this name is not absolute, the range may be different for different cell.

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | int | The according sheet index. |
| row | int | The according row index. |
| column | int | The according column index |

**Returns:** The range.
