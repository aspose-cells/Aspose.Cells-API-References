##ErrorCheckType enumeration
## ErrorCheckType enumeration
Represents all error check type.
The ErrorCheckType type exposes the following members:
### Fields
| Field | Description |
| :- | :- |
| EVALUATION_ERROR | Ignore errors when cells contain formulas that result in an error. |
| CALC |  |
| EMPTY_CELL_REF | Ignore errors when formulas refer to empty cells. |
| NUMBER_STORED_AS_TEXT | Ignore errors when numbers are formatted as text or are preceded by an apostrophe |
| TEXT_NUMBER | Ignore errors when numbers are formatted as text or are preceded by an apostrophe |
| INCONSIST_RANGE | Ignore errors when formulas omit certain cells in a region. |
| INCONSIST_FORMULA | Ignore errors when a formula in a region of your worksheet differs from other formulas in the same region. |
| TWO_DIGIT_TEXT_YEAR | Ignore errors when formulas contain text formatted cells with years represented as 2 digits. |
| TEXT_DATE | Ignore errors when formulas contain text formatted cells with years represented as 2 digits. |
| UNLOCKED_FORMULA | Ignore errors when unlocked cells contain formulas. |
| UNPROCTED_FORMULA | Ignore errors when unlocked cells contain formulas. |
| TABLE_DATA_VALIDATION | Ignore errors when a cell's value in a Table does not comply with the Data Validation rules specified. |
| VALIDATION | Ignore errors when a cell's value in a Table does not comply with the Data Validation rules specified. |
| CALCULATED_COLUMN | Ignore errors when cells contain a value different from a calculated column formula. |
### See Also
* module [`aspose.cells`](..)
