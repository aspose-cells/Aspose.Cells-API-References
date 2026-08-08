---
title: "FormatCondition"
linktitle: "FormatCondition"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents conditional formatting condition."
type: docs
weight: 1600
url: /nodejs/aspose.cells/formatcondition/
---

## FormatCondition class

Represents conditional formatting condition.

## Methods

| Name | Description |
| --- | --- |
| [getAboveAverage()](#getaboveaverage) | Get the conditional formatting's "AboveAverage" instance. The default instance's rule highlights cells that are above th |
| [getColorScale()](#getcolorscale) | Get the conditional formatting's "ColorScale" instance. The default instance is a "green-yellow-red" 3ColorScale . Valid |
| [getDataBar()](#getdatabar) | Get the conditional formatting's "DataBar" instance. The default instance's color is blue. Valid only for type is DataBa |
| [getFormula1()](#getformula1) | Gets and sets the value or expression associated with conditional formatting. Please add all areas before setting formul |
| [getFormula1(isR1C1, isLocal)](#getformula1-1) | Gets the value or expression associated with this format condition. |
| [getFormula1(isR1C1, isLocal, row, column)](#getformula1-2) | Gets the value or expression of the conditional formatting of the cell. The given cell must be contained by this conditi |
| [getFormula1(row, column)](#getformula1-3) | Gets the formula of the conditional formatting of the cell. |
| [getFormula2()](#getformula2) | Gets and sets the value or expression associated with conditional formatting. Please add all areas before setting formul |
| [getFormula2(isR1C1, isLocal)](#getformula2-1) | Gets the value or expression associated with this format condition. |
| [getFormula2(isR1C1, isLocal, row, column)](#getformula2-2) | Gets the value or expression of the conditional formatting of the cell. The given cell must be contained by this conditi |
| [getFormula2(row, column)](#getformula2-3) | Gets the formula of the conditional formatting of the cell. |
| [getIconSet()](#geticonset) | Get the conditional formatting's "IconSet" instance. The default instance's IconSetType is TrafficLights31. Valid only f |
| [getOperator()](#getoperator) | Gets and sets the conditional format operator type. The value of the property is OperatorType integer constant.OperatorT |
| [getPriority()](#getpriority) | The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and r |
| [getStopIfTrue()](#getstopiftrue) | True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. Only applies for Exc |
| [getStyle()](#getstyle) | Gets or setts style of conditional formatted cell ranges. |
| [getText()](#gettext) | The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, be |
| [getTimePeriod()](#gettimeperiod) | The applicable time period in a "date occurring…" conditional formatting rule. Valid only for type = timePeriod. The def |
| [getTop10()](#gettop10) | Get the conditional formatting's "Top10" instance. The default instance's rule highlights cells whose values fall in the |
| [getType()](#gettype) | Gets and sets whether the conditional format Type. The value of the property is FormatConditionType integer constant.For |
| [setFormula1()](#setformula1) | Gets and sets the value or expression associated with conditional formatting. Please add all areas before setting formul |
| [setFormula1(formula, isR1C1, isLocal)](#setformula1-1) | Sets the value or expression associated with this format condition. |
| [setFormula2()](#setformula2) | Gets and sets the value or expression associated with conditional formatting. Please add all areas before setting formul |
| [setFormula2(formula, isR1C1, isLocal)](#setformula2-1) | Sets the value or expression associated with this format condition. |
| [setFormulas(formula1, formula2, isR1C1, isLocal)](#setformulas) | Sets the value or expression associated with this format condition. |
| [setOperator()](#setoperator) | Gets and sets the conditional format operator type. The value of the property is OperatorType integer constant.OperatorT |
| [setPriority()](#setpriority) | The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and r |
| [setStopIfTrue()](#setstopiftrue) | True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. Only applies for Exc |
| [setStyle()](#setstyle) | Gets or setts style of conditional formatted cell ranges. |
| [setText()](#settext) | The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, be |
| [setTimePeriod()](#settimeperiod) | The applicable time period in a "date occurring…" conditional formatting rule. Valid only for type = timePeriod. The def |
| [setType()](#settype) | Gets and sets whether the conditional format Type. The value of the property is FormatConditionType integer constant.For |

### getAboveAverage() {#getaboveaverage}

Get the conditional formatting's "AboveAverage" instance. The default instance's rule highlights cells that are above the average for all values in the range. Valid only for type = AboveAverage.

**Returns:** AboveAverage — `AboveAverage`

### getColorScale() {#getcolorscale}

Get the conditional formatting's "ColorScale" instance. The default instance is a "green-yellow-red" 3ColorScale . Valid only for type = ColorScale.

**Returns:** ColorScale — `ColorScale`

### getDataBar() {#getdatabar}

Get the conditional formatting's "DataBar" instance. The default instance's color is blue. Valid only for type is DataBar.

**Returns:** DataBar — `DataBar`

### getFormula1() {#getformula1}

Gets and sets the value or expression associated with conditional formatting. Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "="=..."".

### getFormula1(isR1C1, isLocal) {#getformula1-1}

Gets the value or expression associated with this format condition.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns:** String — `String` The value or expression associated with this format condition.

### getFormula1(isR1C1, isLocal, row, column) {#getformula1-2}

Gets the value or expression of the conditional formatting of the cell. The given cell must be contained by this conditional formatting, otherwise null will be returned.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
| row | Number | The row index. |
| column | Number | The column index. |

**Returns:** String — `String` The value or expression associated with the conditional formatting of the cell.

### getFormula1(row, column) {#getformula1-3}

Gets the formula of the conditional formatting of the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| column | Number | The column index. |

**Returns:** String — `String` The formula.

### getFormula2() {#getformula2}

Gets and sets the value or expression associated with conditional formatting. Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "="=..."".

### getFormula2(isR1C1, isLocal) {#getformula2-1}

Gets the value or expression associated with this format condition.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns:** String — `String` The value or expression associated with this format condition.

### getFormula2(isR1C1, isLocal, row, column) {#getformula2-2}

Gets the value or expression of the conditional formatting of the cell. The given cell must be contained by this conditional formatting, otherwise null will be returned.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
| row | Number | The row index. |
| column | Number | The column index. |

**Returns:** String — `String` The value or expression associated with the conditional formatting of the cell.

### getFormula2(row, column) {#getformula2-3}

Gets the formula of the conditional formatting of the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Number | The row index. |
| column | Number | The column index. |

**Returns:** String — `String` The formula.

### getIconSet() {#geticonset}

Get the conditional formatting's "IconSet" instance. The default instance's IconSetType is TrafficLights31. Valid only for type = IconSet.

**Returns:** IconSet — `IconSet`

### getOperator() {#getoperator}

Gets and sets the conditional format operator type. The value of the property is OperatorType integer constant.OperatorType

### getPriority() {#getpriority}

The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values, where '1' is the highest priority.

### getStopIfTrue() {#getstopiftrue}

True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. Only applies for Excel 2007;

### getStyle() {#getstyle}

Gets or setts style of conditional formatted cell ranges.

### getText() {#gettext}

The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, beginsWith and endsWith. The default value is null.

### getTimePeriod() {#gettimeperiod}

The applicable time period in a "date occurring…" conditional formatting rule. Valid only for type = timePeriod. The default value is TimePeriodType.Today. The value of the property is TimePeriodType integer constant.

### getTop10() {#gettop10}

Get the conditional formatting's "Top10" instance. The default instance's rule highlights cells whose values fall in the top 10 bracket. Valid only for type is Top10.

**Returns:** Top10 — `Top10`

### getType() {#gettype}

Gets and sets whether the conditional format Type. The value of the property is FormatConditionType integer constant.FormatConditionType

### setFormula1() {#setformula1}

Gets and sets the value or expression associated with conditional formatting. Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "="=..."".

### setFormula1(formula, isR1C1, isLocal) {#setformula1-1}

Sets the value or expression associated with this format condition.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The value or expression associated with this format condition. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "="=..."". |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |

### setFormula2() {#setformula2}

Gets and sets the value or expression associated with conditional formatting. Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "="=..."".

### setFormula2(formula, isR1C1, isLocal) {#setformula2-1}

Sets the value or expression associated with this format condition.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The value or expression associated with this format condition. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "="=..."". |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |

### setFormulas(formula1, formula2, isR1C1, isLocal) {#setformulas}

Sets the value or expression associated with this format condition.

| Parameter | Type | Description |
| --- | --- | --- |
| formula1 | String | The value or expression associated with this format condition. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "="=..."". |
| formula2 | String | The value or expression associated with this format condition. The input format is same with formula1 |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |

### setOperator() {#setoperator}

Gets and sets the conditional format operator type. The value of the property is OperatorType integer constant.OperatorType

### setPriority() {#setpriority}

The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values, where '1' is the highest priority.

### setStopIfTrue() {#setstopiftrue}

True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. Only applies for Excel 2007;

### setStyle() {#setstyle}

Gets or setts style of conditional formatted cell ranges.

### setText() {#settext}

The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, beginsWith and endsWith. The default value is null.

### setTimePeriod() {#settimeperiod}

The applicable time period in a "date occurring…" conditional formatting rule. Valid only for type = timePeriod. The default value is TimePeriodType.Today. The value of the property is TimePeriodType integer constant.

### setType() {#settype}

Gets and sets whether the conditional format Type. The value of the property is FormatConditionType integer constant.FormatConditionType
