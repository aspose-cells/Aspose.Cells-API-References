##Aspose::Cells::ColorScale class
'Aspose::Cells::ColorScale class. Describe the ColorScale conditional formatting rule. This conditional formatting rule creates a gradated color scale on the cells in C++.'
## ColorScale class
Describe the [ColorScale](./) conditional formatting rule. This conditional formatting rule creates a gradated color scale on the cells.
```cpp
class ColorScale
```
## Methods
| Method | Description |
| --- | --- |
| [ColorScale(ColorScale_Impl* impl)](./colorscale/) | Constructs from an implementation object. |
| [ColorScale(const ColorScale\& src)](./colorscale/) | Copy constructor. |
| [GetIs3ColorScale()](./getis3colorscale/) | Indicates whether conditional formatting is 3 color scale. |
| [GetMaxCfvo()](./getmaxcfvo/) | Get or set this [ColorScale](./)'s max value object. Cannot set null or CFValueObject with type [FormatConditionValueType.Min](../formatconditionvaluetype/) to it. |
| [GetMaxColor()](./getmaxcolor/) | Get or set the gradient color for the maximum value in the range. |
| [GetMidCfvo()](./getmidcfvo/) | Get or set this [ColorScale](./)'s mid value object. Cannot set CFValueObject with type [FormatConditionValueType.Max](../formatconditionvaluetype/) or [FormatConditionValueType.Min](../formatconditionvaluetype/) to it. |
| [GetMidColor()](./getmidcolor/) | Get or set the gradient color for the middle value in the range. |
| [GetMinCfvo()](./getmincfvo/) | Get or set this [ColorScale](./)'s min value object. Cannot set null or CFValueObject with type [FormatConditionValueType.Max](../formatconditionvaluetype/) to it. |
| [GetMinColor()](./getmincolor/) | Get or set the gradient color for the minimum value in the range. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ColorScale\& src)](./operator_asm/) | operator= |
| [SetIs3ColorScale(bool value)](./setis3colorscale/) | Indicates whether conditional formatting is 3 color scale. |
| [SetMaxColor(const Aspose::Cells::Color\& value)](./setmaxcolor/) | Get or set the gradient color for the maximum value in the range. |
| [SetMidColor(const Aspose::Cells::Color\& value)](./setmidcolor/) | Get or set the gradient color for the middle value in the range. |
| [SetMinColor(const Aspose::Cells::Color\& value)](./setmincolor/) | Get or set the gradient color for the minimum value in the range. |
| [~ColorScale()](./~colorscale/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
