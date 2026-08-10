---
title: "ReferredArea Class"
linktitle: "ReferredArea"
articleTitle: "ReferredArea"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents a referred area by the formula."
type: docs
weight: 5320
url: /php/aspose.cells/referredarea/
---

## ReferredArea class

Represents a referred area by the formula.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [IsExternalLink](#isexternallink) | boolean | Indicates whether this is an external link. |
| [ExternalFileName](#externalfilename) | String | Get the external file name if this is an external reference. |
| [SheetName](#sheetname) | String | Indicates which sheet this reference is in. |
| [SheetNames](#sheetnames) | String[] |  |
| [IsEntireRow](#isentirerow) | boolean | Indicates whether this area contains all columns(entire row). |
| [IsEntireColumn](#isentirecolumn) | boolean | Indicates whether this area contains all rows(entire column). |
| [IsArea](#isarea) | boolean | Indicates whether this is an area. If this is not an area, only StartRow and StartColumn effect. |
| [EndColumn](#endcolumn) | Number | The end column of the area. |
| [StartColumn](#startcolumn) | Number | The start column of the area. |
| [EndRow](#endrow) | Number | The end row of the area. |
| [StartRow](#startrow) | Number | The start row of the area. |

## Methods

| Name | Description |
| --- | --- |
| [getValues](#getvalues) | Gets cell values in this area. |
| [getValue](#getvalue) | Gets cell value with given offset from the top-left of this area. |
| [toString](#tostring) | Returns the reference address of this area. Generally it is the address of the reference which may be used in formula, s |

### ReferredArea.IsExternalLink property {#isexternallink}

Indicates whether this is an external link.

**Type:** boolean

### ReferredArea.ExternalFileName property {#externalfilename}

Get the external file name if this is an external reference.

**Type:** String

### ReferredArea.SheetName property {#sheetname}

Indicates which sheet this reference is in.

**Type:** String

### ReferredArea.SheetNames property {#sheetnames}

**Type:** String[]

### ReferredArea.IsEntireRow property {#isentirerow}

Indicates whether this area contains all columns(entire row).

**Type:** boolean

### ReferredArea.IsEntireColumn property {#isentirecolumn}

Indicates whether this area contains all rows(entire column).

**Type:** boolean

### ReferredArea.IsArea property {#isarea}

Indicates whether this is an area. If this is not an area, only StartRow and StartColumn effect.

**Type:** boolean

### ReferredArea.EndColumn property {#endcolumn}

The end column of the area.

**Type:** Number

### ReferredArea.StartColumn property {#startcolumn}

The start column of the area.

**Type:** Number

### ReferredArea.EndRow property {#endrow}

The end row of the area.

**Type:** Number

### ReferredArea.StartRow property {#startrow}

The start row of the area.

**Type:** Number

### getValues() (1 of 2) {#getvalues}

Gets cell values in this area.

**Returns:** If this area is invalid, "#REF!" will be returned; If this area is one single cell, then return the cell value object; Otherwise return one 2D array for all values in this area.

---

### getValues(calculateFormulas) (2 of 2) {#getvalues-1}

Gets cell values in this area.

| Parameter | Type | Description |
| --- | --- | --- |
| calculateFormulas | boolean | In this range, if there are some formulas that have not been calculated, this flag denotes whether those formulas should be calculated recursively |

**Returns:** If this area is invalid, "#REF!" will be returned; If this area is one single cell, then return the cell value object; Otherwise return one 2D array for all values in this area.

### getValue(rowOffset, colOffset) (1 of 2) {#getvalue}

Gets cell value with given offset from the top-left of this area.

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Number | row offset from the start row of this area |
| colOffset | Number | column offset from the start row of this area |

**Returns:** "#REF!" if this area is invalid; "#N/A" if given offset out of this area; Otherwise return the cell value at given position.

---

### getValue(rowOffset, colOffset, calculateFormulas) (2 of 2) {#getvalue-1}

Gets cell value with given offset from the top-left of this area.

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Number | row offset from the start row of this area |
| colOffset | Number | column offset from the start row of this area |
| calculateFormulas | boolean | Whether calculate it recursively if the specified reference is formula |

**Returns:** "#REF!" if this area is invalid; "#N/A" if given offset out of this area; Otherwise return the cell value at given position.

### toString() {#tostring}

Returns the reference address of this area. Generally it is the address of the reference which may be used in formula, such as "Sheet1!A1:C3".

**Returns:** the reference address of this area.
