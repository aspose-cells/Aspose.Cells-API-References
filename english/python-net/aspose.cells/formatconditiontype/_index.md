---
title: FormatConditionType
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 4630
url: /python-net/aspose.cells/formatconditiontype/
---

## FormatConditionType enumeration

Conditional format rule type.

## Members
| Member name | Description |
| :- | :- |
|CELL_VALUE|This conditional formatting rule compares a cell value<br/>            to a formula calculated result, using an operator.|
|EXPRESSION|This conditional formatting rule contains a formula to<br/>            evaluate. When the formula result is true, the cell is<br/>            highlighted.|
|COLOR_SCALE|This conditional formatting rule creates a gradated<br/>            color scale on the cells.|
|DATA_BAR|This conditional formatting rule displays a gradated<br/>            data bar in the range of cells.|
|ICON_SET|This conditional formatting rule applies icons to cells<br/>            according to their values.|
|TOP10|This conditional formatting rule highlights cells whose<br/>            values fall in the top N or bottom N bracket, as<br/>            specified.|
|UNIQUE_VALUES|This conditional formatting rule highlights unique<br/>            values in the range.|
|DUPLICATE_VALUES|This conditional formatting rule highlights duplicated<br/>            values.|
|CONTAINS_TEXT|This conditional formatting rule highlights cells<br/>            containing given text. Equivalent to using the SEARCH()<br/>            sheet function to determine whether the cell contains<br/>            the text.|
|NOT_CONTAINS_TEXT|This conditional formatting rule highlights cells that<br/>            do not contain given text. Equivalent of using SEARCH()<br/>            sheet function to determine whether the cell contains<br/>            the text or not.|
|BEGINS_WITH|This conditional formatting rule highlights cells in the<br/>            range that begin with the given text. Equivalent to<br/>            using the LEFT() sheet function and comparing values.|
|ENDS_WITH|This conditional formatting rule highlights cells ending<br/>            with given text. Equivalent to using the RIGHT() sheet<br/>            function and comparing values.|
|CONTAINS_BLANKS|This conditional formatting rule highlights cells that<br/>            are completely blank. Equivalent of using LEN(TRIM()).<br/>            This means that if the cell contains only characters<br/>            that TRIM() would remove, then it is considered blank.<br/>            An empty cell is also considered blank.|
|NOT_CONTAINS_BLANKS|This conditional formatting rule highlights cells that<br/>            are not blank. Equivalent of using LEN(TRIM()). This<br/>            means that if the cell contains only characters that<br/>            TRIM() would remove, then it is considered blank. An<br/>            empty cell is also considered blank.|
|CONTAINS_ERRORS|This conditional formatting rule highlights cells with<br/>            formula errors. Equivalent to using ISERROR() sheet<br/>            function to determine if there is a formula error.|
|NOT_CONTAINS_ERRORS|This conditional formatting rule highlights cells<br/>            without formula errors. Equivalent to using ISERROR()<br/>            sheet function to determine if there is a formula error.|
|TIME_PERIOD|This conditional formatting rule highlights cells<br/>            containing dates in the specified time period. The<br/>            underlying value of the cell is evaluated, therefore the<br/>            cell does not need to be formatted as a date to be<br/>            evaluated. For example, with a cell containing the<br/>            value 38913 the conditional format shall be applied if<br/>            the rule requires a value of 7/14/2006.|
|ABOVE_AVERAGE|This conditional formatting rule highlights cells that<br/>            are above or below the average for all values in the<br/>            range.|

### See Also

* namespace [aspose.cells](/cells/python-net/aspose.cells/)
* assembly [Aspose.Cells](/cells/python-net/)

