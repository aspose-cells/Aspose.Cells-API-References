##ErrorCheckType Enum
'ErrorCheckType enum. Encapsulates the object that represents errorchecktype in Go.'
## ErrorCheckType Enum
Represents all error check type.
```go
type ErrorCheckType int32
```
## Fields
| Field | Description |
| --- | --- |
|[EvaluationError](./evaluationerror/) | Ignore errors when cells contain formulas that result in an error. |
|[EmptyCellRef](./emptycellref/) | Ignore errors when formulas refer to empty cells. |
|[NumberStoredAsText](./numberstoredastext/) | Ignore errors when numbers are formatted as text or are preceded by an apostrophe |
|[InconsistRange](./inconsistrange/) | Ignore errors when formulas omit certain cells in a region. |
|[InconsistFormula](./inconsistformula/) | Ignore errors when a formula in a region of your worksheet differs from other formulas in the same region. |
|[TwoDigitTextYear](./twodigittextyear/) | Ignore errors when formulas contain text formatted cells with years represented as 2 digits. |
|[UnlockedFormula](./unlockedformula/) | Ignore errors when unlocked cells contain formulas. |
|[TableDataValidation](./tabledatavalidation/) | Ignore errors when a cell's value in a Table does not comply with the Data Validation rules specified. |
|[CalculatedColumn](./calculatedcolumn/) | Ignore errors when cells contain a value different from a calculated column formula. |
