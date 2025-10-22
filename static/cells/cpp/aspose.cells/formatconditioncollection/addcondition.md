##Aspose::Cells::FormatConditionCollection::AddCondition method
'Aspose::Cells::FormatConditionCollection::AddCondition method. Adds a formatting condition in C++.'
## FormatConditionCollection::AddCondition(FormatConditionType, OperatorType, const U16String\&, const U16String\&) method
Adds a formatting condition.
```cpp
int32_t Aspose::Cells::FormatConditionCollection::AddCondition(FormatConditionType type, OperatorType operatorType, const U16String &formula1, const U16String &formula2)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | FormatConditionType | The type of format condition. |
| operatorType | OperatorType | The operator type |
| formula1 | const U16String\& | The value or expression associated with conditional formatting. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| formula2 | const U16String\& | The value or expression associated with conditional formatting. The input format is same with formula1 |
## ReturnValue
Formatting condition object index;
## See Also
* Class [Vector](../../vector/)
* Enum [FormatConditionType](../../formatconditiontype/)
* Enum [OperatorType](../../operatortype/)
* Class [U16String](../../u16string/)
* Class [FormatConditionCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## FormatConditionCollection::AddCondition(FormatConditionType, OperatorType, const char16_t*, const char16_t*) method
Adds a formatting condition.
```cpp
int32_t Aspose::Cells::FormatConditionCollection::AddCondition(FormatConditionType type, OperatorType operatorType, const char16_t *formula1, const char16_t *formula2)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | FormatConditionType | The type of format condition. |
| operatorType | OperatorType | The operator type |
| formula1 | const char16_t* | The value or expression associated with conditional formatting. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| formula2 | const char16_t* | The value or expression associated with conditional formatting. The input format is same with formula1 |
## ReturnValue
Formatting condition object index;
## See Also
* Class [Vector](../../vector/)
* Enum [FormatConditionType](../../formatconditiontype/)
* Enum [OperatorType](../../operatortype/)
* Class [FormatConditionCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## FormatConditionCollection::AddCondition(FormatConditionType) method
Add a format condition.
```cpp
int32_t Aspose::Cells::FormatConditionCollection::AddCondition(FormatConditionType type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | FormatConditionType | Format condition type. |
## ReturnValue
Formatting condition object index;
## See Also
* Class [Vector](../../vector/)
* Enum [FormatConditionType](../../formatconditiontype/)
* Class [FormatConditionCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
