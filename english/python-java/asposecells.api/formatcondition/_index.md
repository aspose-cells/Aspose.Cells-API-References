---
title: "FormatCondition Class"
linktitle: "FormatCondition"
articleTitle: "FormatCondition"
second_title: "Aspose.Cells for Python via Java"
description: "Represents conditional formatting condition."
type: docs
weight: 2540
url: /python-java/asposecells.api/formatcondition/
---

## FormatCondition class

Represents conditional formatting condition.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Formula1](#formula1) | String | Gets and sets the value or expression associated with conditional formatting. Please add all areas before setting formul |
| [Formula2](#formula2) | String | Gets and sets the value or expression associated with conditional formatting. Please add all areas before setting formul |
| [Operator](#operator) | int | Gets and sets the conditional format operator type. The value of the property is OperatorType integer constant. |
| [StopIfTrue](#stopiftrue) | boolean | True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. Only applies for Exc |
| [Priority](#priority) | int | The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and r |
| [Style](#style) | Style | Gets or setts style of conditional formatted cell ranges. |
| [Type](#type) | int | Gets and sets whether the conditional format Type. The value of the property is FormatConditionType integer constant. |
| [IconSet](#iconset) | IconSet | Get the conditional formatting's "IconSet" instance. The default instance's IconSetType is TrafficLights31. Valid only f |
| [DataBar](#databar) | DataBar | Get the conditional formatting's "DataBar" instance. The default instance's color is blue. Valid only for type is DataBa |
| [ColorScale](#colorscale) | ColorScale | Get the conditional formatting's "ColorScale" instance. The default instance is a "green-yellow-red" 3ColorScale . Valid |
| [Top10](#top10) | Top10 | Get the conditional formatting's "Top10" instance. The default instance's rule highlights cells whose values fall in the |
| [AboveAverage](#aboveaverage) | AboveAverage | Get the conditional formatting's "AboveAverage" instance. The default instance's rule highlights cells that are above th |
| [Text](#text) | String | The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, be |
| [TimePeriod](#timeperiod) | int | The applicable time period in a "date occurring…" conditional formatting rule. Valid only for type = timePeriod. The def |

## Methods

| Name | Description |
| --- | --- |
| [getFormula1](#getformula1) | Gets the value or expression associated with this format condition. |
| [getFormula2](#getformula2) | Gets the value or expression associated with this format condition. |
| [setFormulas](#setformulas) | Sets the value or expression associated with this format condition. |
| [setFormula1](#setformula1) | Sets the value or expression associated with this format condition. |
| [setFormula2](#setformula2) | Sets the value or expression associated with this format condition. |

### FormatCondition.Formula1 property {#formula1}

Gets and sets the value or expression associated with conditional formatting. Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"".

**Type:** String

### FormatCondition.Formula2 property {#formula2}

Gets and sets the value or expression associated with conditional formatting. Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"".

**Type:** String

### FormatCondition.Operator property {#operator}

Gets and sets the conditional format operator type. The value of the property is OperatorType integer constant.

**Type:** int

### FormatCondition.StopIfTrue property {#stopiftrue}

True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. Only applies for Excel 2007;

**Type:** boolean

### FormatCondition.Priority property {#priority}

The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values, where '1' is the highest priority.

**Type:** int

### FormatCondition.Style property {#style}

Gets or setts style of conditional formatted cell ranges.

**Type:** Style

### FormatCondition.Type property {#type}

Gets and sets whether the conditional format Type. The value of the property is FormatConditionType integer constant.

**Type:** int

### FormatCondition.IconSet property {#iconset}

Get the conditional formatting's "IconSet" instance. The default instance's IconSetType is TrafficLights31. Valid only for type = IconSet.

**Type:** IconSet

### FormatCondition.DataBar property {#databar}

Get the conditional formatting's "DataBar" instance. The default instance's color is blue. Valid only for type is DataBar.

**Type:** DataBar

### FormatCondition.ColorScale property {#colorscale}

Get the conditional formatting's "ColorScale" instance. The default instance is a "green-yellow-red" 3ColorScale . Valid only for type = ColorScale.

**Type:** ColorScale

### FormatCondition.Top10 property {#top10}

Get the conditional formatting's "Top10" instance. The default instance's rule highlights cells whose values fall in the top 10 bracket. Valid only for type is Top10.

**Type:** Top10

### FormatCondition.AboveAverage property {#aboveaverage}

Get the conditional formatting's "AboveAverage" instance. The default instance's rule highlights cells that are above the average for all values in the range. Valid only for type = AboveAverage.

**Type:** AboveAverage

### FormatCondition.Text property {#text}

The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, beginsWith and endsWith. The default value is null.

**Type:** String

### FormatCondition.TimePeriod property {#timeperiod}

The applicable time period in a "date occurring…" conditional formatting rule. Valid only for type = timePeriod. The default value is TimePeriodType.Today. The value of the property is TimePeriodType integer constant.

**Type:** int

### getFormula1(isR1C1, isLocal) (1 of 3) {#getformula1}

Gets the value or expression associated with this format condition.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns:** The value or expression associated with this format condition.

---

### getFormula1(isR1C1, isLocal, row, column) (2 of 3) {#getformula1-1}

Gets the value or expression of the conditional formatting of the cell.

The given cell must be contained by this conditional formatting, otherwise null will be returned.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
| row | int | The row index. |
| column | int | The column index. |

**Returns:** The value or expression associated with the conditional formatting of the cell.

---

### getFormula1(row, column) (3 of 3) {#getformula1-2}

Gets the formula of the conditional formatting of the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |
| column | int | The column index. |

**Returns:** The formula.

### getFormula2(isR1C1, isLocal) (1 of 3) {#getformula2}

Gets the value or expression associated with this format condition.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns:** The value or expression associated with this format condition.

---

### getFormula2(isR1C1, isLocal, row, column) (2 of 3) {#getformula2-1}

Gets the value or expression of the conditional formatting of the cell.

The given cell must be contained by this conditional formatting, otherwise null will be returned.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
| row | int | The row index. |
| column | int | The column index. |

**Returns:** The value or expression associated with the conditional formatting of the cell.

---

### getFormula2(row, column) (3 of 3) {#getformula2-2}

Gets the formula of the conditional formatting of the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |
| column | int | The column index. |

**Returns:** The formula.

### setFormulas(formula1, formula2, isR1C1, isLocal) {#setformulas}

Sets the value or expression associated with this format condition.

| Parameter | Type | Description |
| --- | --- | --- |
| formula1 | String | The value or expression associated with this format condition. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| formula2 | String | The value or expression associated with this format condition. The input format is same with formula1 |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |

### setFormula1(formula, isR1C1, isLocal) {#setformula1}

Sets the value or expression associated with this format condition.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The value or expression associated with this format condition. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |

### setFormula2(formula, isR1C1, isLocal) {#setformula2}

Sets the value or expression associated with this format condition.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The value or expression associated with this format condition. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |
