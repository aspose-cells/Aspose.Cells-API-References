##Aspose::Cells::FormatCondition::SetFormulas method
'Aspose::Cells::FormatCondition::SetFormulas method. Sets the value or expression associated with this format condition in C++.'
## FormatCondition::SetFormulas(const U16String\&, const U16String\&, bool, bool) method
Sets the value or expression associated with this format condition.
```cpp
void Aspose::Cells::FormatCondition::SetFormulas(const U16String &formula1, const U16String &formula2, bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula1 | const U16String\& | The value or expression associated with this format condition. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| formula2 | const U16String\& | The value or expression associated with this format condition. The input format is same with formula1 |
| isR1C1 | bool | Whether the formula is R1C1 formula. |
| isLocal | bool | Whether the formula is locale formatted. |
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [FormatCondition](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## FormatCondition::SetFormulas(const char16_t*, const char16_t*, bool, bool) method
Sets the value or expression associated with this format condition.
```cpp
void Aspose::Cells::FormatCondition::SetFormulas(const char16_t *formula1, const char16_t *formula2, bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula1 | const char16_t* | The value or expression associated with this format condition. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| formula2 | const char16_t* | The value or expression associated with this format condition. The input format is same with formula1 |
| isR1C1 | bool | Whether the formula is R1C1 formula. |
| isLocal | bool | Whether the formula is locale formatted. |
## See Also
* Class [Vector](../../vector/)
* Class [FormatCondition](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
