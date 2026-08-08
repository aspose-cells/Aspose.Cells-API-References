---
title: "Name"
linktitle: "Name"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents a defined name for a range of cells."
type: docs
weight: 2310
url: /nodejs/aspose.cells/name/
---

## Name class

Represents a defined name for a range of cells.

## Methods

| Name | Description |
| --- | --- |
| [getComment()](#getcomment) | Gets and sets the comment of the name. Only applies for Excel 2007 or higher versions. |
| [getFullText()](#getfulltext) | Gets the name full text of the object with the scope setting. |
| [getR1C1RefersTo()](#getr1c1refersto) | Gets or sets a R1C1 reference of the Name. |
| [getRange()](#getrange) | Gets the range if this name refers to a range. |
| [getRange(recalculate)](#getrange-1) | Gets the range if this name refers to a range |
| [getRange(sheetIndex, row, column)](#getrange-2) | Gets the range if this name refers to a range. If the reference of this name is not absolute, the range may be different |
| [getRanges()](#getranges) | Gets all ranges referred by this name. |
| [getRanges(recalculate)](#getranges-1) | Gets all ranges referred by this name. |
| [getReferredAreas(recalculate)](#getreferredareas) | Gets all references referred by this name. |
| [getRefersTo()](#getrefersto) | Returns or sets the formula that the name is defined to refer to, beginning with an equal sign. |
| [getRefersTo(isR1C1, isLocal)](#getrefersto-1) | Get the reference of this Name. |
| [getRefersTo(isR1C1, isLocal, row, column)](#getrefersto-2) | Get the reference of this Name based on specified cell. |
| [getSheetIndex()](#getsheetindex) | Indicates this name belongs to Workbook or Worksheet. 0 = Global name, otherwise index to sheet (one-based) |
| [getText()](#gettext) | Gets the name text of the object. |
| [isReferred()](#isreferred) | Indicates whether this name is referred by other formulas. |
| [isVisible()](#isvisible) | Indicates whether the name is visible. |
| [setComment()](#setcomment) | Gets and sets the comment of the name. Only applies for Excel 2007 or higher versions. |
| [setR1C1RefersTo()](#setr1c1refersto) | Gets or sets a R1C1 reference of the Name. |
| [setRefersTo()](#setrefersto) | Returns or sets the formula that the name is defined to refer to, beginning with an equal sign. |
| [setRefersTo(refersTo, isR1C1, isLocal)](#setrefersto-1) | Set the reference of this Name. |
| [setSheetIndex()](#setsheetindex) | Indicates this name belongs to Workbook or Worksheet. 0 = Global name, otherwise index to sheet (one-based) |
| [setText()](#settext) | Gets the name text of the object. |
| [setVisible()](#setvisible) | Indicates whether the name is visible. |
| [toString()](#tostring) | Returns a string represents the current Range object. |

### getComment() {#getcomment}

Gets and sets the comment of the name. Only applies for Excel 2007 or higher versions.

### getFullText() {#getfulltext}

Gets the name full text of the object with the scope setting.

### getR1C1RefersTo() {#getr1c1refersto}

Gets or sets a R1C1 reference of the Name.

### getRange() {#getrange}

Gets the range if this name refers to a range.

**Returns:** Range — `Range` The range.

### getRange(recalculate) {#getrange-1}

Gets the range if this name refers to a range

| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | boolean | whether recalculate it if this name has been calculated before this invocation. |

**Returns:** Range — `Range` The range.

### getRange(sheetIndex, row, column) {#getrange-2}

Gets the range if this name refers to a range. If the reference of this name is not absolute, the range may be different for different cell.

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Number | The according sheet index. |
| row | Number | The according row index. |
| column | Number | The according column index |

**Returns:** Range — `Range` The range.

### getRanges() {#getranges}

Gets all ranges referred by this name.

**Returns:** Array ofRange — `Array ofRange` All ranges.

### getRanges(recalculate) {#getranges-1}

Gets all ranges referred by this name.

| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | boolean | whether recalculate it if this name has been calculated before this invocation. |

**Returns:** Array ofRange — `Array ofRange` All ranges.

### getReferredAreas(recalculate) {#getreferredareas}

Gets all references referred by this name.

| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | boolean | whether recalculate it if this name has been calculated before this invocation. |

**Returns:** Array ofReferredArea — `Array ofReferredArea` All ranges.

### getRefersTo() {#getrefersto}

Returns or sets the formula that the name is defined to refer to, beginning with an equal sign.

### getRefersTo(isR1C1, isLocal) {#getrefersto-1}

Get the reference of this Name.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the reference needs to be formatted as R1C1. |
| isLocal | boolean | Whether the reference needs to be formatted by locale. |

### getRefersTo(isR1C1, isLocal, row, column) {#getrefersto-2}

Get the reference of this Name based on specified cell.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the reference needs to be formatted as R1C1. |
| isLocal | boolean | Whether the reference needs to be formatted by locale. |
| row | Number | The row index of the cell. |
| column | Number | The column index of the cell. |

### getSheetIndex() {#getsheetindex}

Indicates this name belongs to Workbook or Worksheet. 0 = Global name, otherwise index to sheet (one-based)

### getText() {#gettext}

Gets the name text of the object.

### isReferred() {#isreferred}

Indicates whether this name is referred by other formulas.

### isVisible() {#isvisible}

Indicates whether the name is visible.

### setComment() {#setcomment}

Gets and sets the comment of the name. Only applies for Excel 2007 or higher versions.

### setR1C1RefersTo() {#setr1c1refersto}

Gets or sets a R1C1 reference of the Name.

### setRefersTo() {#setrefersto}

Returns or sets the formula that the name is defined to refer to, beginning with an equal sign.

### setRefersTo(refersTo, isR1C1, isLocal) {#setrefersto-1}

Set the reference of this Name.

| Parameter | Type | Description |
| --- | --- | --- |
| refersTo | String | The reference. |
| isR1C1 | boolean | Whether the reference is R1C1 format. |
| isLocal | boolean | Whether the reference is locale formatted. |

### setSheetIndex() {#setsheetindex}

Indicates this name belongs to Workbook or Worksheet. 0 = Global name, otherwise index to sheet (one-based)

### setText() {#settext}

Gets the name text of the object.

### setVisible() {#setvisible}

Indicates whether the name is visible.

### toString() {#tostring}

Returns a string represents the current Range object.

**Returns:** String — `String`
