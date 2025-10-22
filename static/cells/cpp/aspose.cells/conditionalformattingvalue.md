##Aspose::Cells::ConditionalFormattingValue class
'Aspose::Cells::ConditionalFormattingValue class. Describes the values of the interpolation points in a gradient scale, dataBar or iconSet in C++.'
## ConditionalFormattingValue class
Describes the values of the interpolation points in a gradient scale, dataBar or iconSet.
```cpp
class ConditionalFormattingValue
```
## Methods
| Method | Description |
| --- | --- |
| [ConditionalFormattingValue(ConditionalFormattingValue_Impl* impl)](./conditionalformattingvalue/) | Constructs from an implementation object. |
| [ConditionalFormattingValue(const ConditionalFormattingValue\& src)](./conditionalformattingvalue/) | Copy constructor. |
| [GetType()](./gettype/) | Get or set the type of this conditional formatting value object. Setting the type to [FormatConditionValueType.Min](../formatconditionvaluetype/) or [FormatConditionValueType.Max](../formatconditionvaluetype/) will auto set "Value" to null. |
| [GetValue()](./getvalue/) | Get or set the value of this conditional formatting value object. It should be used in conjunction with Type. |
| [IsGTE()](./isgte/) | Get or set the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the greater than or equal to operator. 'false' indicates 'greater than' is used instead of 'greater than or equal to'. Default value is true. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ConditionalFormattingValue\& src)](./operator_asm/) | operator= |
| [SetIsGTE(bool value)](./setisgte/) | Get or set the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the greater than or equal to operator. 'false' indicates 'greater than' is used instead of 'greater than or equal to'. Default value is true. |
| [SetType(FormatConditionValueType value)](./settype/) | Get or set the type of this conditional formatting value object. Setting the type to [FormatConditionValueType.Min](../formatconditionvaluetype/) or [FormatConditionValueType.Max](../formatconditionvaluetype/) will auto set "Value" to null. |
| [SetValue(const Aspose::Cells::Object\& value)](./setvalue/) | Get or set the value of this conditional formatting value object. It should be used in conjunction with Type. |
| [~ConditionalFormattingValue()](./~conditionalformattingvalue/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
