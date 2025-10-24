##FormatConditionType Enum
'FormatConditionType enum. Encapsulates the object that represents formatconditiontype in Go.'
## FormatConditionType Enum
Conditional format rule type.
```go
type FormatConditionType int32
```
## Fields
| Field | Description |
| --- | --- |
|[CellValue](./cellvalue/) | This conditional formatting rule compares a cell valueto a formula calculated result, using an operator. |
|[Expression](./expression/) | This conditional formatting rule contains a formula toevaluate. When the formula result is true, the cell ishighlighted. |
|[Top10](./top10/) | This conditional formatting rule highlights cells whosevalues fall in the top N or bottom N bracket, asspecified. |
|[UniqueValues](./uniquevalues/) | This conditional formatting rule highlights uniquevalues in the range. |
|[DuplicateValues](./duplicatevalues/) | This conditional formatting rule highlights duplicatedvalues. |
|[ContainsText](./containstext/) | This conditional formatting rule highlights cellscontaining given text. Equivalent to using the SEARCH()sheet function to determine whether the cell containsthe text. |
|[NotContainsText](./notcontainstext/) | This conditional formatting rule highlights cells thatdo not contain given text. Equivalent of using SEARCH()sheet function to determine whether the cell containsthe text or not. |
|[BeginsWith](./beginswith/) | This conditional formatting rule highlights cells in therange that begin with the given text. Equivalent tousing the LEFT() sheet function and comparing values. |
|[EndsWith](./endswith/) | This conditional formatting rule highlights cells endingwith given text. Equivalent to using the RIGHT() sheetfunction and comparing values. |
|[ContainsBlanks](./containsblanks/) | This conditional formatting rule highlights cells thatare completely blank. Equivalent of using LEN(TRIM()).This means that if the cell contains only charactersthat TRIM() would remove, then it is considered blank.An empty cell is also considered blank. |
|[NotContainsBlanks](./notcontainsblanks/) | This conditional formatting rule highlights cells thatare not blank. Equivalent of using LEN(TRIM()). Thismeans that if the cell contains only characters thatTRIM() would remove, then it is considered blank. Anempty cell is also considered blank. |
|[ContainsErrors](./containserrors/) | This conditional formatting rule highlights cells withformula errors. Equivalent to using ISERROR() sheetfunction to determine if there is a formula error. |
|[NotContainsErrors](./notcontainserrors/) | This conditional formatting rule highlights cellswithout formula errors. Equivalent to using ISERROR()sheet function to determine if there is a formula error. |
|[TimePeriod](./timeperiod/) | This conditional formatting rule highlights cellscontaining dates in the specified time period. Theunderlying value of the cell is evaluated, therefore thecell does not need to be formatted as a date to beevaluated. For example, with a cell containing thevalue 38913 the conditional format shall be applied ifthe rule requires a value of 7/14/2006. |
|[AboveAverage](./aboveaverage/) | This conditional formatting rule highlights cells thatare above or below the average for all values in therange. |
|[ColorScale](./colorscale/) | This conditional formatting rule creates a gradatedcolor scale on the cells. |
|[DataBar](./databar/) | This conditional formatting rule displays a gradateddata bar in the range of cells. |
|[IconSet](./iconset/) | This conditional formatting rule applies icons to cellsaccording to their values. |
