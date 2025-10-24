##Aspose::Cells::Style::SetCustom method
'Aspose::Cells::Style::SetCustom method. Sets the Custom number format string of a cell in C++.'
## Style::SetCustom(const U16String\&, bool) method
Sets the Custom number format string of a cell.
```cpp
void Aspose::Cells::Style::SetCustom(const U16String &custom, bool builtinPreference)
```
| Parameter | Type | Description |
| --- | --- | --- |
| custom | const U16String\& | Custom number format string, should be InvariantCulture pattern. |
| builtinPreference | bool | If given Custom number format string matches one of the built-in number formats corresponding to current regional settings, whether set the number format as built-in instead of Custom. |
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [Style](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Style::SetCustom(const char16_t*, bool) method
Sets the Custom number format string of a cell.
```cpp
void Aspose::Cells::Style::SetCustom(const char16_t *custom, bool builtinPreference)
```
| Parameter | Type | Description |
| --- | --- | --- |
| custom | const char16_t* | Custom number format string, should be InvariantCulture pattern. |
| builtinPreference | bool | If given Custom number format string matches one of the built-in number formats corresponding to current regional settings, whether set the number format as built-in instead of Custom. |
## See Also
* Class [Vector](../../vector/)
* Class [Style](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Style::SetCustom(const U16String\&) method
Represents the custom number format string of this style object. If the custom number format is not set(For example, the number format is builtin), "" will be returned.
```cpp
void Aspose::Cells::Style::SetCustom(const U16String &value)
```
## Remarks
The returned custom string is culture-independent.
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [Style](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Style::SetCustom(const char16_t*) method
Represents the custom number format string of this style object. If the custom number format is not set(For example, the number format is builtin), "" will be returned.
```cpp
void Aspose::Cells::Style::SetCustom(const char16_t *value)
```
## Remarks
The returned custom string is culture-independent.
## See Also
* Class [Vector](../../vector/)
* Class [Style](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
