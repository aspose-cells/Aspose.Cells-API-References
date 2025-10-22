##FormatConditionType
Conditional format rule type.
## FormatConditionType enumeration
Conditional format rule type.
### Values
| Name | Value | Description |
| --- | --- | --- |
| CellValue | `1` | This conditional formatting rule compares a cell value to a formula calculated result, using an operator. |
| Expression | `2` | This conditional formatting rule contains a formula to evaluate. When the formula result is true, the cell is highlighted. |
| Top10 | `4` | This conditional formatting rule highlights cells whose values fall in the top N or bottom N bracket, as specified. |
| UniqueValues | `8` | This conditional formatting rule highlights unique values in the range. |
| DuplicateValues | `16` | This conditional formatting rule highlights duplicated values. |
| ContainsText | `32` | This conditional formatting rule highlights cells containing given text. Equivalent to using the SEARCH() sheet function to determine whether the cell contains the text. |
| NotContainsText | `64` | This conditional formatting rule highlights cells that do not contain given text. Equivalent of using SEARCH() sheet function to determine whether the cell contains the text or not. |
| BeginsWith | `128` | This conditional formatting rule highlights cells in the range that begin with the given text. Equivalent to using the LEFT() sheet function and comparing values. |
| EndsWith | `256` | This conditional formatting rule highlights cells ending with given text. Equivalent to using the RIGHT() sheet function and comparing values. |
| ContainsBlanks | `512` | This conditional formatting rule highlights cells that are completely blank. Equivalent of using LEN(TRIM()). This means that if the cell contains only characters that TRIM() would remove, then it is considered blank. An empty cell is also considered blank. |
| NotContainsBlanks | `1024` | This conditional formatting rule highlights cells that are not blank. Equivalent of using LEN(TRIM()). This means that if the cell contains only characters that TRIM() would remove, then it is considered blank. An empty cell is also considered blank. |
| ContainsErrors | `2048` | This conditional formatting rule highlights cells with formula errors. Equivalent to using ISERROR() sheet function to determine if there is a formula error. |
| NotContainsErrors | `4096` | This conditional formatting rule highlights cells without formula errors. Equivalent to using ISERROR() sheet function to determine if there is a formula error. |
| TimePeriod | `8192` | This conditional formatting rule highlights cells containing dates in the specified time period. The underlying value of the cell is evaluated, therefore the cell does not need to be formatted as a date to be evaluated. For example, with a cell containing the value 38913 the conditional format shall be applied if the rule requires a value of 7/14/2006. |
| AboveAverage | `16384` | This conditional formatting rule highlights cells that are above or below the average for all values in the range. |
| ColorScale | `32768` | This conditional formatting rule creates a gradated color scale on the cells. |
| DataBar | `65536` | This conditional formatting rule displays a gradated data bar in the range of cells. |
| IconSet | `131072` | This conditional formatting rule applies icons to cells according to their values. |
