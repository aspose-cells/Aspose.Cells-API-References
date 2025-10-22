##Aspose::Cells::LookInType enum
'Aspose::Cells::LookInType enum. Represents look in type in C++.'
## LookInType enum
Represents look in type.
```cpp
enum class LookInType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Formulas | 0 | <br>Finds the searched object from formula(Cell.Formula) if the cell is formula, otherwise finds from cell's original value(same with [OriginalValues](./)). |
| Values | 1 | <br>Finds object from cell's original value(Cell.Value) and formatted value(Cell.StringValue). |
| ValuesExcludeFormulaCell | 2 | <br>Ignores cells that are formula. For those cells that are not formula, it is same with [Values](../autofilltype/). |
| Comments | 3 | <br>Finds object from cell's comment only. Ignores those cells that have no comment. |
| OnlyFormulas | 4 | <br>Ignores cells that are not formula. For those cells that are formula, finds the searched object from formula(Cell.Formula). |
| OriginalValues | 5 | <br>Find object from cell's original value only. |
| FormattedValues | 6 | <br>Find object from cell's formatted value(Cell.StringValue) only. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
