---
title: Aspose::Cells::FontConfigs class
linktitle: FontConfigs
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::FontConfigs class. Specifies font settings in C++.'
type: docs
weight: 6800
url: /cpp/aspose.cells/fontconfigs/
---
## FontConfigs class


Specifies font settings.

```cpp
class FontConfigs
```

## Methods

| Method | Description |
| --- | --- |
| [FontConfigs()](./fontconfigs/) | Default constructor. |
| [FontConfigs(FontConfigs_Impl* impl)](./fontconfigs/) | Constructs from an implementation object. |
| [FontConfigs(const FontConfigs\& src)](./fontconfigs/) | Copy constructor. |
| static [GetDefaultFontName()](./getdefaultfontname/) | Gets or sets the default font name. |
| static [GetFontFileDataInfo(const U16String\& fontName, bool isBold, bool isItalic, bool isExactStyle)](./getfontfiledatainfo/) | Get data information of font file data. |
| static [GetFontFileDataInfo(const char16_t* fontName, bool isBold, bool isItalic, bool isExactStyle)](./getfontfiledatainfo/) | Get data information of font file data. |
| static [GetFontSources()](./getfontsources/) | Gets a copy of the array that contains the list of sources. |
| static [GetFontSubstitutes(const U16String\& originalFontName)](./getfontsubstitutes/) | Returns an array containing font substitute names to be used if original font is not present. |
| static [GetFontSubstitutes(const char16_t* originalFontName)](./getfontsubstitutes/) | Returns an array containing font substitute names to be used if original font is not present. |
| static [GetPreferSystemFontSubstitutes()](./getprefersystemfontsubstitutes/) | Indicate whether to use system font substitutes first or not when a font is not presented and the substitute of this font is not set. e.g. On Ubuntu, "Arial" font is generally substituted by "Liberation Sans". Default value is false. |
| static [IsFontAvailable(const U16String\& fontName)](./isfontavailable/) | Indicate whether the font is available. |
| static [IsFontAvailable(const char16_t* fontName)](./isfontavailable/) | Indicate whether the font is available. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const FontConfigs\& src)](./operator_asm/) | operator= |
| static [SetDefaultFontName(const U16String\& value)](./setdefaultfontname/) | Gets or sets the default font name. |
| static [SetDefaultFontName(const char16_t* value)](./setdefaultfontname/) | Gets or sets the default font name. |
| static [SetFontFolder(const U16String\& fontFolder, bool recursive)](./setfontfolder/) | Sets the fonts folder. |
| static [SetFontFolder(const char16_t* fontFolder, bool recursive)](./setfontfolder/) | Sets the fonts folder. |
| static [SetFontFolders(const Vector \<U16String\>\& fontFolders, bool recursive)](./setfontfolders/) | Sets the fonts folder. |
| static [SetFontSources(const Vector \<FontSourceBase\>\& sources)](./setfontsources/) | Sets the font sources. |
| static [SetFontSubstitutes(const U16String\& originalFontName, const Vector \<U16String\>\& substituteFontNames)](./setfontsubstitutes/) | [Font](../font/) substitute names for given original font name. |
| static [SetFontSubstitutes(const char16_t* originalFontName, const Vector \<U16String\>\& substituteFontNames)](./setfontsubstitutes/) | [Font](../font/) substitute names for given original font name. |
| static [SetPreferSystemFontSubstitutes(bool value)](./setprefersystemfontsubstitutes/) | Indicate whether to use system font substitutes first or not when a font is not presented and the substitute of this font is not set. e.g. On Ubuntu, "Arial" font is generally substituted by "Liberation Sans". Default value is false. |
| [~FontConfigs()](./~fontconfigs/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
