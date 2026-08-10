---
title: "FormatConditionType Enum"
linktitle: "FormatConditionType"
articleTitle: "FormatConditionType"
second_title: "Aspose.Cells for Python via Java"
description: "Utility class containing constants."
type: docs
weight: 2560
url: /python-java/asposecells.api/formatconditiontype/
---

## FormatConditionType enumeration

Utility class containing constants. Conditional format rule type.

## Values

| Name | Description |
| --- | --- |
| CELL_VALUE | This conditional formatting rule compares a cell value to a formula calculated result, using an operator. |
| EXPRESSION | This conditional formatting rule contains a formula to evaluate. When the formula result is true, the cell is highlighted. |
| TOP_10 | This conditional formatting rule highlights cells whose values fall in the top N or bottom N bracket, as specified. |
| UNIQUE_VALUES | This conditional formatting rule highlights unique values in the range. |
| DUPLICATE_VALUES | This conditional formatting rule highlights duplicated values. |
| CONTAINS_TEXT | This conditional formatting rule highlights cells containing given text. Equivalent to using the SEARCH() sheet function to determine whether the cell contains the text. |
| NOT_CONTAINS_TEXT | This conditional formatting rule highlights cells that do not contain given text. Equivalent of using SEARCH() sheet function to determine whether the cell contains the text or not. |
| BEGINS_WITH | This conditional formatting rule highlights cells in the range that begin with the given text. Equivalent to using the LEFT() sheet function and comparing values. |
| ENDS_WITH | This conditional formatting rule highlights cells ending with given text. Equivalent to using the RIGHT() sheet function and comparing values. |
| CONTAINS_BLANKS | This conditional formatting rule highlights cells that are completely blank. Equivalent of using LEN(TRIM()). This means that if the cell contains only characters that TRIM() would remove, then it is considered blank. An empty cell is also considered blank. |
| NOT_CONTAINS_BLANKS | This conditional formatting rule highlights cells that are not blank. Equivalent of using LEN(TRIM()). This means that if the cell contains only characters that TRIM() would remove, then it is considered blank. An empty cell is also considered blank. |
| CONTAINS_ERRORS | This conditional formatting rule highlights cells with formula errors. Equivalent to using ISERROR() sheet function to determine if there is a formula error. |
| NOT_CONTAINS_ERRORS | This conditional formatting rule highlights cells without formula errors. Equivalent to using ISERROR() sheet function to determine if there is a formula error. |
| TIME_PERIOD | This conditional formatting rule highlights cells containing dates in the specified time period. The underlying value of the cell is evaluated, therefore the cell does not need to be formatted as a date to be evaluated. For example, with a cell containing the value 38913 the conditional format shall be applied if the rule requires a value of 7/14/2006. |
| ABOVE_AVERAGE | This conditional formatting rule highlights cells that are above or below the average for all values in the range. |
| COLOR_SCALE | This conditional formatting rule creates a gradated color scale on the cells. |
| DATA_BAR | This conditional formatting rule displays a gradated data bar in the range of cells. |
| ICON_SET | This conditional formatting rule applies icons to cells according to their values. |
