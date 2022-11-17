---
title: FormatCondition
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 690
url: /python-net/aspose.cells/formatcondition/
---

## FormatCondition class

Represents conditional formatting condition.

The FormatCondition type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|formula1|Gets and sets the value or expression associated with conditional formatting.|
|formula2|Gets and sets the value or expression associated with conditional formatting.|
|operator|Gets and sets the conditional format operator type.|
|stop_if_true|True, no rules with lower priority may be applied over this rule, when this rule evaluates to true.<br/>            Only applies for Excel 2007;|
|priority|The priority of this conditional formatting rule. This value is used to determine which<br/>            format should be evaluated and rendered. Lower numeric values are higher priority than<br/>            higher numeric values, where '1' is the highest priority.|
|style|Gets or setts style of conditional formatted cell ranges.|
|type|Gets and sets whether the conditional format Type.|
|icon_set|Get the conditional formatting's "IconSet" instance.<br/>            The default instance's IconSetType is TrafficLights31.<br/>            Valid only for type = IconSet.|
|data_bar|Get the conditional formatting's "DataBar" instance.<br/>            The default instance's color is blue.<br/>            Valid only for type is DataBar.|
|color_scale|Get the conditional formatting's "ColorScale" instance.<br/>            The default instance is a "green-yellow-red" 3ColorScale .<br/>            Valid only for type = ColorScale.|
|top10|Get the conditional formatting's "Top10" instance.<br/>            The default instance's rule highlights cells whose<br/>            values fall in the top 10 bracket.<br/>            Valid only for type is Top10.|
|above_average|Get the conditional formatting's "AboveAverage" instance.<br/>            The default instance's rule highlights cells that are <br/>            above the average for all values in the range.<br/>            Valid only for type = AboveAverage.|
|text|The text value in a "text contains" conditional formatting rule. <br/>            Valid only for type = containsText, notContainsText, beginsWith and endsWith.<br/>            The default value is null.|
|time_period|The applicable time period in a "date occurring…" conditional formatting rule. <br/>            Valid only for type = timePeriod.<br/>            The default value is TimePeriodType.Today.|
## Methods
| Name | Description |
| :- | :- |
|get_formula1(is_r1c1, is_local)|Gets the value or expression associated with this format condition.|
|get_formula1(is_r1c1, is_local, row, column)|Gets the value or expression of the conditional formatting of the cell.|
|get_formula1(row, column)|Gets the value or expression of the conditional formatting of the cell.|
|get_formula2(is_r1c1, is_local)|Gets the value or expression associated with this format condition.|
|get_formula2(is_r1c1, is_local, row, column)|Gets the value or expression of the conditional formatting of the cell.|
|get_formula2(row, column)|Gets the value or expression of the conditional formatting of the cell.|
|set_formulas(formula1, formula2, is_r1c1, is_local)|Sets the value or expression associated with this format condition.|
|set_formula1(formula, is_r1c1, is_local)|Sets the value or expression associated with this format condition.|
|set_formula2(formula, is_r1c1, is_local)|Sets the value or expression associated with this format condition.|

### See Also

* namespace [aspose.cells](/cells/python-net/aspose.cells/)
* assembly [Aspose.Cells](/cells/python-net/)

