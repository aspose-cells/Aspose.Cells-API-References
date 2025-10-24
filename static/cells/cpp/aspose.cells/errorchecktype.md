##Aspose::Cells::ErrorCheckType enum
'Aspose::Cells::ErrorCheckType enum. Represents all error check type in C++.'
## ErrorCheckType enum
Represents all error check type.
```cpp
enum class ErrorCheckType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| EvaluationError | 1 | <br>Ignore errors when cells contain formulas that result in an error. |
| Calc | 1 |  **(Deprecated - Use ErrorCheckType.EvaluationError instead. )** <br> |
| EmptyCellRef | 2 | <br>Ignore errors when formulas refer to empty cells. |
| NumberStoredAsText | 4 | <br>Ignore errors when numbers are formatted as text or are preceded by an apostrophe. |
| TextNumber | 4 |  **(Deprecated - Use ErrorCheckType.NumberStoredAsText instead. )** <br>Ignore errors when numbers are formatted as text or are preceded by an apostrophe. |
| InconsistRange | 8 | <br>Ignore errors when formulas omit certain cells in a region. |
| InconsistFormula | 16 | <br>Ignore errors when a formula in a region of your worksheet differs from other formulas in the same region. |
| TwoDigitTextYear | 32 | <br>Ignore errors when formulas contain text formatted cells with years represented as 2 digits. |
| TextDate | 32 |  **(Deprecated - Use ErrorCheckType.TwoDigitTextYear instead. )** <br>Ignore errors when formulas contain text formatted cells with years represented as 2 digits. |
| UnlockedFormula | 64 | <br>Ignore errors when unlocked cells contain formulas. |
| UnproctedFormula | 64 |  **(Deprecated - Use ErrorCheckType.UnproctedFormula instead. )** <br>Ignore errors when unlocked cells contain formulas. |
| TableDataValidation | 128 | <br>Ignore errors when a cell's value in a Table does not comply with the Data [Validation](../validation/) rules specified. |
| Validation | 128 |  **(Deprecated - Use ErrorCheckType.TableDataValidation instead. )** <br>Ignore errors when a cell's value in a Table does not comply with the Data [Validation](../validation/) rules specified. |
| CalculatedColumn | 129 | <br>Ignore errors when cells contain a value different from a calculated column formula. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
