---
title: "ListColumn Class"
linktitle: "ListColumn"
articleTitle: "ListColumn"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents a column in a Table."
type: docs
weight: 3420
url: /php/aspose.cells/listcolumn/
---

## ListColumn class

Represents a column in a Table.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Name](#name) | String | Gets and sets the name of the column. If sets the name of the column, the according cell' value will be changed too. |
| [TotalsCalculation](#totalscalculation) | Number | Gets and sets the type of calculation in the Totals row of the list column. The value of the property is TotalsCalculati |
| [Range](#range) | Range | Gets the range of this list column. |
| [IsArrayFormula](#isarrayformula) | boolean |  |
| [Formula](#formula) | String | Gets and sets the formula of the list column. |
| [TotalsRowLabel](#totalsrowlabel) | String | Gets and sets the display labels of total row. |

## Methods

| Name | Description |
| --- | --- |
| [getCustomTotalsRowFormula](#getcustomtotalsrowformula) | Gets the formula of totals row of this list column. |
| [setCustomTotalsRowFormula](#setcustomtotalsrowformula) | Gets the formula of totals row of this list column. |
| [getCustomCalculatedFormula](#getcustomcalculatedformula) | Gets the formula of this list column. |
| [setCustomCalculatedFormula](#setcustomcalculatedformula) | Sets the formula for this list column. |
| [getDataStyle](#getdatastyle) | Gets the style of the data in this column of the table. |
| [setDataStyle](#setdatastyle) | Sets the style of the data in this column of the table. |

### ListColumn.Name property {#name}

Gets and sets the name of the column. If sets the name of the column, the according cell' value will be changed too.

**Type:** String

### ListColumn.TotalsCalculation property {#totalscalculation}

Gets and sets the type of calculation in the Totals row of the list column. The value of the property is TotalsCalculation integer constant.

**Type:** Number

### ListColumn.Range property {#range}

Gets the range of this list column.

**Type:** Range

### ListColumn.IsArrayFormula property {#isarrayformula}

**Type:** boolean

### ListColumn.Formula property {#formula}

Gets and sets the formula of the list column.

**Type:** String

### ListColumn.TotalsRowLabel property {#totalsrowlabel}

Gets and sets the display labels of total row.

**Type:** String

### getCustomTotalsRowFormula(isR1C1, isLocal) {#getcustomtotalsrowformula}

Gets the formula of totals row of this list column.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns:** The formula of this list column.

### setCustomTotalsRowFormula(formula, isR1C1, isLocal) {#setcustomtotalsrowformula}

Gets the formula of totals row of this list column.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | the formula for this list column. |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

### getCustomCalculatedFormula(isR1C1, isLocal) {#getcustomcalculatedformula}

Gets the formula of this list column.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns:** The formula of this list column.

### setCustomCalculatedFormula(formula, isR1C1, isLocal) {#setcustomcalculatedformula}

Sets the formula for this list column.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | the formula for this list column. |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

### getDataStyle() {#getdatastyle}

Gets the style of the data in this column of the table.

### setDataStyle(style) {#setdatastyle}

Sets the style of the data in this column of the table.
