##Aspose::Cells::Drawing::ShapeCollection::AddTextEffectInChart method
'Aspose::Cells::Drawing::ShapeCollection::AddTextEffectInChart method. Inserts a WordArt object to the chart in C++.'
## ShapeCollection::AddTextEffectInChart(MsoPresetTextEffect, const U16String\&, const U16String\&, int32_t, bool, bool, int32_t, int32_t, int32_t, int32_t) method
Inserts a WordArt object to the chart.
```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::AddTextEffectInChart(MsoPresetTextEffect effect, const U16String &text, const U16String &fontName, int32_t size, bool fontBold, bool fontItalic, int32_t top, int32_t left, int32_t height, int32_t width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| effect | MsoPresetTextEffect | The mso preset text effect type. |
| text | const U16String\& | The WordArt text. |
| fontName | const U16String\& | The font name. |
| size | int32_t | The font size |
| fontBold | bool | Indicates whether font is bold. |
| fontItalic | bool | Indicates whether font is italic. |
| top | int32_t | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| left | int32_t | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| height | int32_t | Represents the height of shape, in units of 1/4000 of the chart area. |
| width | int32_t | Represents the width of shape, in units of 1/4000 of the chart area. |
## ReturnValue
Returns a [Shape](../../shape/) object that represents the new WordArt object.
## See Also
* Class [Shape](../../shape/)
* Enum [MsoPresetTextEffect](../../msopresettexteffect/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## ShapeCollection::AddTextEffectInChart(MsoPresetTextEffect, const char16_t*, const char16_t*, int32_t, bool, bool, int32_t, int32_t, int32_t, int32_t) method
Inserts a WordArt object to the chart.
```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::AddTextEffectInChart(MsoPresetTextEffect effect, const char16_t *text, const char16_t *fontName, int32_t size, bool fontBold, bool fontItalic, int32_t top, int32_t left, int32_t height, int32_t width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| effect | MsoPresetTextEffect | The mso preset text effect type. |
| text | const char16_t* | The WordArt text. |
| fontName | const char16_t* | The font name. |
| size | int32_t | The font size |
| fontBold | bool | Indicates whether font is bold. |
| fontItalic | bool | Indicates whether font is italic. |
| top | int32_t | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| left | int32_t | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| height | int32_t | Represents the height of shape, in units of 1/4000 of the chart area. |
| width | int32_t | Represents the width of shape, in units of 1/4000 of the chart area. |
## ReturnValue
Returns a [Shape](../../shape/) object that represents the new WordArt object.
## See Also
* Class [Shape](../../shape/)
* Enum [MsoPresetTextEffect](../../msopresettexteffect/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
