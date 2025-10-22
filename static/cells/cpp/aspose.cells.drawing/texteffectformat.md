##Aspose::Cells::Drawing::TextEffectFormat class
'Aspose::Cells::Drawing::TextEffectFormat class. Contains properties and methods that apply to WordArt objects in C++.'
## TextEffectFormat class
Contains properties and methods that apply to WordArt objects.
```cpp
class TextEffectFormat
```
## Methods
| Method | Description |
| --- | --- |
| [GetFontBold()](./getfontbold/) | Indicates whether font is bold. |
| [GetFontItalic()](./getfontitalic/) | Indicates whether font is italic. |
| [GetFontName()](./getfontname/) | The name of the font used in the WordArt. |
| [GetFontSize()](./getfontsize/) | The size (in points) of the font used in the WordArt. |
| [GetPresetShape()](./getpresetshape/) | Gets and sets the preset shape type. |
| [GetRotatedChars()](./getrotatedchars/) | If true,characters in the specified WordArt are rotated 90 degrees relative to the WordArt's bounding shape. |
| [GetText()](./gettext/) | The text in the WordArt. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const TextEffectFormat\& src)](./operator_asm/) | operator= |
| [SetFontBold(bool value)](./setfontbold/) | Indicates whether font is bold. |
| [SetFontItalic(bool value)](./setfontitalic/) | Indicates whether font is italic. |
| [SetFontName(const U16String\& value)](./setfontname/) | The name of the font used in the WordArt. |
| [SetFontName(const char16_t* value)](./setfontname/) | The name of the font used in the WordArt. |
| [SetFontSize(int32_t value)](./setfontsize/) | The size (in points) of the font used in the WordArt. |
| [SetPresetShape(MsoPresetTextEffectShape value)](./setpresetshape/) | Gets and sets the preset shape type. |
| [SetRotatedChars(bool value)](./setrotatedchars/) | If true,characters in the specified WordArt are rotated 90 degrees relative to the WordArt's bounding shape. |
| [SetText(const U16String\& value)](./settext/) | The text in the WordArt. |
| [SetText(const char16_t* value)](./settext/) | The text in the WordArt. |
| [SetTextEffect(MsoPresetTextEffect effect)](./settexteffect/) | Sets the preset text effect. |
| [TextEffectFormat(TextEffectFormat_Impl* impl)](./texteffectformat/) | Constructs from an implementation object. |
| [TextEffectFormat(const TextEffectFormat\& src)](./texteffectformat/) | Copy constructor. |
| [~TextEffectFormat()](./~texteffectformat/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
ShapeCollection shapes = workbook.GetWorksheets().Get(0).GetShapes();
shapes.AddTextEffect(MsoPresetTextEffect::TextEffect1, u"Aspose", u"Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
TextEffectFormat textEffectFormat = shapes.Get(0).GetTextEffect();
textEffectFormat.SetTextEffect(MsoPresetTextEffect::TextEffect10);
workbook.Save(u"Book1.xls");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Drawing](../)
* Library [Aspose.Cells for C++](../../)
