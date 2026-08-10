---
title: "FormatConditionCollection Class"
linktitle: "FormatConditionCollection"
articleTitle: "FormatConditionCollection"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents conditional formatting."
type: docs
weight: 2550
url: /php/aspose.cells/formatconditioncollection/
---

## FormatConditionCollection class

Represents conditional formatting. The FormatConditions can contain up to three conditional formats.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | Number | Gets the count of the conditions. |
| [RangeCount](#rangecount) | Number | Gets count of conditionally formatted ranges. |
| [Item (int)](#itemint) | FormatCondition | Gets the formatting condition by index. |

## Methods

| Name | Description |
| --- | --- |
| [add](#add) | Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three  |
| [addArea](#addarea) | Adds a conditional formatted cell range. |
| [addCondition](#addcondition) | Adds a formatting condition. |
| [getCellArea](#getcellarea) | Gets the conditional formatted cell range by index. |
| [removeArea](#removearea) | Removes conditional formatted cell range by index. |
| [removeCondition](#removecondition) | Removes the formatting condition by index. |

### FormatConditionCollection.Count property {#count}

Gets the count of the conditions.

**Type:** Number

### FormatConditionCollection.RangeCount property {#rangecount}

Gets count of conditionally formatted ranges.

**Type:** Number

### FormatConditionCollection.Item (int) property {#itemint}

Gets the formatting condition by index.

**Type:** FormatCondition

### add(cellArea, type, operatorType, formula1, formula2) {#add}

Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats. References to the other sheets are not allowed in the formulas of conditional formatting.

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | Conditional formatted cell range. |
| type | Number | A FormatConditionType value. Type of conditional formatting.It could be one of the members of FormatConditionType. |
| operatorType | Number | A OperatorType value. Comparison operator.It could be one of the members of OperatorType. |
| formula1 | String | The value or expression associated with conditional formatting. |
| formula2 | String | The value or expression associated with conditional formatting |

**Returns:** [0]:Formatting condition object index;[1] Effected cell rang index.

### addArea(cellArea) {#addarea}

Adds a conditional formatted cell range.

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | Conditional formatted cell range. |

**Returns:** Conditional formatted cell rang index.

### addCondition(type, operatorType, formula1, formula2) (1 of 2) {#addcondition}

Adds a formatting condition.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | A FormatConditionType value. The type of format condition. |
| operatorType | Number | A OperatorType value. The operator type |
| formula1 | String | The value or expression associated with conditional formatting. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| formula2 | String | The value or expression associated with conditional formatting. The input format is same with formula1 |

**Returns:** Formatting condition object index;

---

### addCondition(type) (2 of 2) {#addcondition-1}

Add a format condition.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | A FormatConditionType value. Format condition type. |

**Returns:** Formatting condition object index;

### getCellArea(index) {#getcellarea}

Gets the conditional formatted cell range by index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | the index of the conditional formatted cell range. |

**Returns:** the conditional formatted cell range

### removeArea(index) (1 of 2) {#removearea}

Removes conditional formatted cell range by index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index of the conditional formatted cell range to be removed. |

---

### removeArea(startRow, startColumn, totalRows, totalColumns) (2 of 2) {#removearea-1}

Remove conditional formatting int the range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | The startRow of the range. |
| startColumn | Number | The startColumn of the range. |
| totalRows | Number | The number of rows of the range. |
| totalColumns | Number | The number of columns of the range. |

**Returns:** Returns TRUE, this FormatCondtionCollection should be removed.

### removeCondition(index) {#removecondition}

Removes the formatting condition by index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index of the formatting condition to be removed. |
