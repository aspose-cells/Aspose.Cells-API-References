##Aspose::Cells::Worksheet::ConvertFormulaReferenceStyle method
'Aspose::Cells::Worksheet::ConvertFormulaReferenceStyle method. Converts the formula reference style in C++.'
## Worksheet::ConvertFormulaReferenceStyle(const U16String\&, bool, int32_t, int32_t) method
Converts the formula reference style.
```cpp
U16String Aspose::Cells::Worksheet::ConvertFormulaReferenceStyle(const U16String &formula, bool toR1C1, int32_t baseCellRow, int32_t baseCellColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const U16String\& | The formula to be converted. |
| toR1C1 | bool | Which reference style to convert the formula to. If the original formula is of A1 reference style, then this value should be true so the formula will be converted from A1 to R1C1 reference style; If the original formula is of R1C1 reference style, then this value should be false so the formula will be converted from R1C1 to A1 reference style; |
| baseCellRow | int32_t | The row index of the base cell. |
| baseCellColumn | int32_t | The column index of the base cell. |
## ReturnValue
The converted formula.
## See Also
* Class [U16String](../../u16string/)
* Class [Vector](../../vector/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Worksheet::ConvertFormulaReferenceStyle(const char16_t*, bool, int32_t, int32_t) method
Converts the formula reference style.
```cpp
U16String Aspose::Cells::Worksheet::ConvertFormulaReferenceStyle(const char16_t *formula, bool toR1C1, int32_t baseCellRow, int32_t baseCellColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const char16_t* | The formula to be converted. |
| toR1C1 | bool | Which reference style to convert the formula to. If the original formula is of A1 reference style, then this value should be true so the formula will be converted from A1 to R1C1 reference style; If the original formula is of R1C1 reference style, then this value should be false so the formula will be converted from R1C1 to A1 reference style; |
| baseCellRow | int32_t | The row index of the base cell. |
| baseCellColumn | int32_t | The column index of the base cell. |
## ReturnValue
The converted formula.
## See Also
* Class [U16String](../../u16string/)
* Class [Vector](../../vector/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
