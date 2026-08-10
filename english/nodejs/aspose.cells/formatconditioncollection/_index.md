---
title: "FormatConditionCollection"
linktitle: "FormatConditionCollection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents conditional formatting."
type: docs
weight: 1610
url: /nodejs/aspose.cells/formatconditioncollection/
---

## FormatConditionCollection class

Represents conditional formatting. The FormatConditions can contain up to three conditional formats.

## Methods

| Name | Description |
| --- | --- |
| [add(cellArea, type, operatorType, formula1, formula2)](#add) | Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three  |
| [addArea(cellArea)](#addarea) | Adds a conditional formatted cell range. |
| [addCondition(type, operatorType, formula1, formula2)](#addcondition) | Adds a formatting condition. |
| [addCondition(type)](#addcondition-1) | Add a format condition. |
| [get(index)](#get) | Gets the formatting condition by index. |
| [getCellArea(index)](#getcellarea) | Gets the conditional formatted cell range by index. |
| [getCount()](#getcount) | Gets the count of the conditions. |
| [getRangeCount()](#getrangecount) | Gets count of conditionally formatted ranges. |
| [removeArea(index)](#removearea) | Removes conditional formatted cell range by index. |
| [removeArea(startRow, startColumn, totalRows, totalColumns)](#removearea-1) | Remove conditional formatting int the range. |
| [removeCondition(index)](#removecondition) | Removes the formatting condition by index. |

### add(cellArea, type, operatorType, formula1, formula2) {#add}

Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats. References to the other sheets are not allowed in the formulas of conditional formatting. OperatorType

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | Conditional formatted cell range. |
| type | Number | FormatConditionType |
| operatorType | Number | OperatorType |
| formula1 | String | The value or expression associated with conditional formatting. |
| formula2 | String | The value or expression associated with conditional formatting |

**Returns:** Array of Number — `Array of Number` [0]:Formatting condition object index;[1] Effected cell rang index.

### addArea(cellArea) {#addarea}

Adds a conditional formatted cell range.

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | Conditional formatted cell range. |

**Returns:** Number — `Number` Conditional formatted cell rang index.

### addCondition(type, operatorType, formula1, formula2) {#addcondition}

Adds a formatting condition.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | FormatConditionType |
| operatorType | Number | OperatorType |
| formula1 | String | The value or expression associated with conditional formatting. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "="=..."". |
| formula2 | String | The value or expression associated with conditional formatting. The input format is same with formula1 |

**Returns:** Number — `Number` Formatting condition object index;

### addCondition(type) {#addcondition-1}

Add a format condition.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | FormatConditionType |

**Returns:** Number — `Number` Formatting condition object index;

### get(index) {#get}

Gets the formatting condition by index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | the index of the formatting condition to return. |

**Returns:** FormatCondition — `FormatCondition` the formatting condition

### getCellArea(index) {#getcellarea}

Gets the conditional formatted cell range by index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | the index of the conditional formatted cell range. |

**Returns:** CellArea — `CellArea` the conditional formatted cell range

### getCount() {#getcount}

Gets the count of the conditions.

### getRangeCount() {#getrangecount}

Gets count of conditionally formatted ranges.

### removeArea(index) {#removearea}

Removes conditional formatted cell range by index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index of the conditional formatted cell range to be removed. |

### removeArea(startRow, startColumn, totalRows, totalColumns) {#removearea-1}

Remove conditional formatting int the range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | The startRow of the range. |
| startColumn | Number | The startColumn of the range. |
| totalRows | Number | The number of rows of the range. |
| totalColumns | Number | The number of columns of the range. |

**Returns:** boolean — `boolean` Returns TRUE, this FormatCondtionCollection should be removed.

### removeCondition(index) {#removecondition}

Removes the formatting condition by index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index of the formatting condition to be removed. |
