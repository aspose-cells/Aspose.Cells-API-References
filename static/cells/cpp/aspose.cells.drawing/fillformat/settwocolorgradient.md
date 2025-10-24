##Aspose::Cells::Drawing::FillFormat::SetTwoColorGradient method
'Aspose::Cells::Drawing::FillFormat::SetTwoColorGradient method. Sets the specified fill to a two-color gradient. Only applies for Excel 2007 in C++.'
## FillFormat::SetTwoColorGradient(const Aspose::Cells::Color\&, const Aspose::Cells::Color\&, GradientStyleType, int32_t) method
Sets the specified fill to a two-color gradient. Only applies for Excel 2007.
```cpp
void Aspose::Cells::Drawing::FillFormat::SetTwoColorGradient(const Aspose::Cells::Color &color1, const Aspose::Cells::Color &color2, GradientStyleType style, int32_t variant)
```
| Parameter | Type | Description |
| --- | --- | --- |
| color1 | const Aspose::Cells::Color\& | One gradient color. |
| color2 | const Aspose::Cells::Color\& | Two gradient color. |
| style | GradientStyleType | Gradient shading style. |
| variant | int32_t | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Enum [GradientStyleType](../../gradientstyletype/)
* Class [FillFormat](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## FillFormat::SetTwoColorGradient(const Aspose::Cells::Color\&, double, const Aspose::Cells::Color\&, double, GradientStyleType, int32_t) method
Sets the specified fill to a two-color gradient. Only applies for Excel 2007.
```cpp
void Aspose::Cells::Drawing::FillFormat::SetTwoColorGradient(const Aspose::Cells::Color &color1, double transparency1, const Aspose::Cells::Color &color2, double transparency2, GradientStyleType style, int32_t variant)
```
| Parameter | Type | Description |
| --- | --- | --- |
| color1 | const Aspose::Cells::Color\& | One gradient color. |
| transparency1 | double | The degree of transparency of the color1 as a value from 0.0 (opaque) through 1.0 (clear). |
| color2 | const Aspose::Cells::Color\& | Two gradient color. |
| transparency2 | double | The degree of transparency of the color2 as a value from 0.0 (opaque) through 1.0 (clear). |
| style | GradientStyleType | Gradient shading style. |
| variant | int32_t | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Enum [GradientStyleType](../../gradientstyletype/)
* Class [FillFormat](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
