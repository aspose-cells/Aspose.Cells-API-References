---
title: "ReferredArea"
linktitle: "ReferredArea"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents a referred area by the formula."
type: docs
weight: 3160
url: /nodejs/aspose.cells/referredarea/
---

## ReferredArea class

Represents a referred area by the formula.

## Methods

| Name | Description |
| --- | --- |
| [getEndColumn()](#getendcolumn) | The end column of the area. |
| [getEndRow()](#getendrow) | The end row of the area. |
| [getExternalFileName()](#getexternalfilename) | Get the external file name if this is an external reference. |
| [getSheetName()](#getsheetname) | Indicates which sheet this reference is in. |
| [getSheetNames()](#getsheetnames) |  |
| [getStartColumn()](#getstartcolumn) | The start column of the area. |
| [getStartRow()](#getstartrow) | The start row of the area. |
| [getValue(rowOffset, colOffset)](#getvalue) | Gets cell value with given offset from the top-left of this area. |
| [getValue(rowOffset, colOffset, calculateFormulas)](#getvalue-1) | Gets cell value with given offset from the top-left of this area. |
| [getValues()](#getvalues) | Gets cell values in this area. |
| [getValues(calculateFormulas)](#getvalues-1) | Gets cell values in this area. |
| [isArea()](#isarea) | Indicates whether this is an area. If this is not an area, only StartRow and StartColumn effect. |
| [isEntireColumn()](#isentirecolumn) | Indicates whether this area contains all rows(entire column). |
| [isEntireRow()](#isentirerow) | Indicates whether this area contains all columns(entire row). |
| [isExternalLink()](#isexternallink) | Indicates whether this is an external link. |
| [toString()](#tostring) | Returns the reference address of this area. Generally it is the address of the reference which may be used in formula, s |

### getEndColumn() {#getendcolumn}

The end column of the area.

### getEndRow() {#getendrow}

The end row of the area.

### getExternalFileName() {#getexternalfilename}

Get the external file name if this is an external reference.

### getSheetName() {#getsheetname}

Indicates which sheet this reference is in.

### getSheetNames() {#getsheetnames}

### getStartColumn() {#getstartcolumn}

The start column of the area.

### getStartRow() {#getstartrow}

The start row of the area.

### getValue(rowOffset, colOffset) {#getvalue}

Gets cell value with given offset from the top-left of this area.

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Number | row offset from the start row of this area |
| colOffset | Number | column offset from the start row of this area |

**Returns:** Object — `Object` "#REF!" if this area is invalid; "#N/A" if given offset out of this area; Otherwise return the cell value at given position.

### getValue(rowOffset, colOffset, calculateFormulas) {#getvalue-1}

Gets cell value with given offset from the top-left of this area.

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Number | row offset from the start row of this area |
| colOffset | Number | column offset from the start row of this area |
| calculateFormulas | boolean | Whether calculate it recursively if the specified reference is formula |

**Returns:** Object — `Object` "#REF!" if this area is invalid; "#N/A" if given offset out of this area; Otherwise return the cell value at given position.

### getValues() {#getvalues}

Gets cell values in this area.

**Returns:** Object — `Object` If this area is invalid, "#REF!" will be returned; If this area is one single cell, then return the cell value object; Otherwise return one 2D array for all values in this area.

### getValues(calculateFormulas) {#getvalues-1}

Gets cell values in this area.

| Parameter | Type | Description |
| --- | --- | --- |
| calculateFormulas | boolean | In this range, if there are some formulas that have not been calculated, this flag denotes whether those formulas should be calculated recursively |

**Returns:** Object — `Object` If this area is invalid, "#REF!" will be returned; If this area is one single cell, then return the cell value object; Otherwise return one 2D array for all values in this area.

### isArea() {#isarea}

Indicates whether this is an area. If this is not an area, only StartRow and StartColumn effect.

### isEntireColumn() {#isentirecolumn}

Indicates whether this area contains all rows(entire column).

### isEntireRow() {#isentirerow}

Indicates whether this area contains all columns(entire row).

### isExternalLink() {#isexternallink}

Indicates whether this is an external link.

### toString() {#tostring}

Returns the reference address of this area. Generally it is the address of the reference which may be used in formula, such as "Sheet1!A1:C3".

**Returns:** String — `String` the reference address of this area.
