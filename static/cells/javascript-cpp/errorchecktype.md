##ErrorCheckType
Represents all error check type.
## ErrorCheckType enumeration
Represents all error check type.
### Values
| Name | Value | Description |
| --- | --- | --- |
| EvaluationError | `1` | Ignore errors when cells contain formulas that result in an error. |
| Calc | `1` |  |
| EmptyCellRef | `2` | Ignore errors when formulas refer to empty cells. |
| NumberStoredAsText | `4` | Ignore errors when numbers are formatted as text or are preceded by an apostrophe |
| TextNumber | `4` | Ignore errors when numbers are formatted as text or are preceded by an apostrophe |
| InconsistRange | `8` | Ignore errors when formulas omit certain cells in a region. |
| InconsistFormula | `16` | Ignore errors when a formula in a region of your worksheet differs from other formulas in the same region. |
| TwoDigitTextYear | `32` | Ignore errors when formulas contain text formatted cells with years represented as 2 digits. |
| TextDate | `32` | Ignore errors when formulas contain text formatted cells with years represented as 2 digits. |
| UnlockedFormula | `64` | Ignore errors when unlocked cells contain formulas. |
| UnproctedFormula | `64` | Ignore errors when unlocked cells contain formulas. |
| TableDataValidation | `128` | Ignore errors when a cell's value in a Table does not comply with the Data Validation rules specified. |
| Validation | `128` | Ignore errors when a cell's value in a Table does not comply with the Data Validation rules specified. |
| CalculatedColumn | `129` | Ignore errors when cells contain a value different from a calculated column formula. |
