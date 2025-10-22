##Aspose::Cells::FormatCondition::GetFormula2 method
'Aspose::Cells::FormatCondition::GetFormula2 method. Gets the value or expression associated with this format condition in C++.'
## FormatCondition::GetFormula2(bool, bool) method
Gets the value or expression associated with this format condition.
```cpp
U16String Aspose::Cells::FormatCondition::GetFormula2(bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | bool | Whether the formula needs to be formatted as R1C1. |
| isLocal | bool | Whether the formula needs to be formatted by locale. |
## ReturnValue
The value or expression associated with this format condition.
## See Also
* Class [U16String](../../u16string/)
* Class [Vector](../../vector/)
* Class [FormatCondition](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## FormatCondition::GetFormula2(bool, bool, int32_t, int32_t) method
Gets the value or expression of the conditional formatting of the cell.
```cpp
U16String Aspose::Cells::FormatCondition::GetFormula2(bool isR1C1, bool isLocal, int32_t row, int32_t column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | bool | Whether the formula needs to be formatted as R1C1. |
| isLocal | bool | Whether the formula needs to be formatted by locale. |
| row | int32_t | The row index. |
| column | int32_t | The column index. |
## ReturnValue
The value or expression associated with the conditional formatting of the cell.
## Remarks
The given cell must be contained by this conditional formatting, otherwise null will be returned.
## See Also
* Class [U16String](../../u16string/)
* Class [Vector](../../vector/)
* Class [FormatCondition](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## FormatCondition::GetFormula2() method
Gets and sets the value or expression associated with conditional formatting.
```cpp
U16String Aspose::Cells::FormatCondition::GetFormula2()
```
## Remarks
Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"".
## See Also
* Class [U16String](../../u16string/)
* Class [FormatCondition](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## FormatCondition::GetFormula2(int32_t, int32_t) method
Gets the formula of the conditional formatting of the cell.
```cpp
U16String Aspose::Cells::FormatCondition::GetFormula2(int32_t row, int32_t column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | int32_t | The row index. |
| column | int32_t | The column index. |
## ReturnValue
The formula.
## See Also
* Class [U16String](../../u16string/)
* Class [Vector](../../vector/)
* Class [FormatCondition](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
