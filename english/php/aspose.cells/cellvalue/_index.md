---
title: "CellValue Class"
linktitle: "CellValue"
articleTitle: "CellValue"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents the cell value and corresponding type."
type: docs
weight: 570
url: /php/aspose.cells/cellvalue/
---

## CellValue class

Represents the cell value and corresponding type.

## Constructors

| Name | Description |
| --- | --- |
| [CellValue](#constructor) |  |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Type](#type) | Number | Gets/sets the type of cell value. The value of the property is CellValueType integer constant. |
| [Value](#value) | Object | Gets/sets the cell value. The value must be of the correct type of object corresponding to the Type : Type Value CellVal |

### CellValue() {#constructor}

### CellValue.Type property {#type}

Gets/sets the type of cell value. The value of the property is CellValueType integer constant.

**Type:** Number

### CellValue.Value property {#value}

Gets/sets the cell value. The value must be of the correct type of object corresponding to the Type : Type Value CellValueType.IS_NULL null, any other object will be ignored CellValueType.IS_NUMERIC double CellValueType.IS_DATE_TIME DateTime CellValueType.IS_STRING string CellValueType.IS_BOOL bool CellValueType.IS_ERROR error string such as "#VALUE!", "#NAME?", ...

**Type:** Object
