##Enum FormatConditionType
Aspose.Cells.GridDesktop.FormatConditionType enum. Conditional format rule type
## FormatConditionType enumeration
Conditional format rule type.
```csharp
public enum FormatConditionType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| CellValue | `0` | This conditional formatting rule compares a cell value to a formula calculated result, using an operator. |
| Expression | `1` | This conditional formatting rule contains a formula to evaluate. When the formula result is true, the cell is highlighted. |
| ColorScale | `2` | This conditional formatting rule creates a gradated color scale on the cells. |
| DataBar | `3` | This conditional formatting rule displays a gradated data bar in the range of cells. |
| IconSet | `4` | This conditional formatting rule applies icons to cells according to their values. |
| Top10 | `5` | This conditional formatting rule highlights cells whose values fall in the top N or bottom N bracket, as specified. |
| UniqueValues | `6` | This conditional formatting rule highlights unique values in the range. |
| DuplicateValues | `7` | This conditional formatting rule highlights duplicated values. |
| ContainsText | `8` | This conditional formatting rule highlights cells containing given text. Equivalent to using the SEARCH() sheet function to determine whether the cell contains the text. |
| NotContainsText | `9` | This conditional formatting rule highlights cells that are not blank. Equivalent of using LEN(TRIM()). This means that if the cell contains only characters that TRIM() would remove, then it is considered blank. An empty cell is also considered blank. |
| BeginsWith | `10` | This conditional formatting rule highlights cells in the range that begin with the given text. Equivalent to using the LEFT() sheet function and comparing values. |
| EndsWith | `11` | This conditional formatting rule highlights cells ending with given text. Equivalent to using the RIGHT() sheet function and comparing values. |
| ContainsBlanks | `12` | This conditional formatting rule highlights cells that are completely blank. Equivalent of using LEN(TRIM()). This means that if the cell contains only characters that TRIM() would remove, then it is considered blank. An empty cell is also considered blank. |
| NotContainsBlanks | `13` | This conditional formatting rule highlights cells that are not blank. Equivalent of using LEN(TRIM()). This means that if the cell contains only characters that TRIM() would remove, then it is considered blank. An empty cell is also considered blank. |
| ContainsErrors | `14` | This conditional formatting rule highlights cells with formula errors. Equivalent to using ISERROR() sheet function to determine if there is a formula error. |
| NotContainsErrors | `15` | This conditional formatting rule highlights cells without formula errors. Equivalent to using ISERROR() sheet function to determine if there is a formula error. |
| TimePeriod | `16` | This conditional formatting rule highlights cells containing dates in the specified time period. The underlying value of the cell is evaluated, therefore the cell does not need to be formatted as a date to be evaluated. For example, with a cell containing the value 38913 the conditional format shall be applied if the rule requires a value of 7/14/2006. |
| AboveAverage | `17` | This conditional formatting rule highlights cells that are above or below the average for all values in the range. |
### See Also
* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)
