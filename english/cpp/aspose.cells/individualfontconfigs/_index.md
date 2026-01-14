---
title: Aspose::Cells::IndividualFontConfigs class
linktitle: IndividualFontConfigs
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::IndividualFontConfigs class. Font configs for each Workbook object in C++.'
type: docs
weight: 9100
url: /cpp/aspose.cells/individualfontconfigs/
---
## IndividualFontConfigs class


[Font](../font/) configs for each [Workbook](../workbook/) object.

```cpp
class IndividualFontConfigs
```

## Methods

| Method | Description |
| --- | --- |
| [GetFontSources()](./getfontsources/) | Gets a copy of the array that contains the list of sources. |
| [GetFontSubstitutes(const U16String\& originalFontName)](./getfontsubstitutes/) | Returns an array containing font substitute names to be used if original font is not presented. |
| [GetFontSubstitutes(const char16_t* originalFontName)](./getfontsubstitutes/) | Returns an array containing font substitute names to be used if original font is not presented. |
| [IndividualFontConfigs()](./individualfontconfigs/) | Ctor. |
| [IndividualFontConfigs(IndividualFontConfigs_Impl* impl)](./individualfontconfigs/) | Constructs from an implementation object. |
| [IndividualFontConfigs(const IndividualFontConfigs\& src)](./individualfontconfigs/) | Copy constructor. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const IndividualFontConfigs\& src)](./operator_asm/) | operator= |
| [SetFontFolder(const U16String\& fontFolder, bool recursive)](./setfontfolder/) | Sets the fonts folder. |
| [SetFontFolder(const char16_t* fontFolder, bool recursive)](./setfontfolder/) | Sets the fonts folder. |
| [SetFontFolders(const Vector \<U16String\>\& fontFolders, bool recursive)](./setfontfolders/) | Sets the font folders. |
| [SetFontSources(const Vector \<FontSourceBase\>\& sources)](./setfontsources/) | Sets the font sources. |
| [SetFontSubstitutes(const U16String\& originalFontName, const Vector \<U16String\>\& substituteFontNames)](./setfontsubstitutes/) | Sets font substitute names for a given original font name. |
| [SetFontSubstitutes(const char16_t* originalFontName, const Vector \<U16String\>\& substituteFontNames)](./setfontsubstitutes/) | Sets font substitute names for a given original font name. |
| [~IndividualFontConfigs()](./~individualfontconfigs/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
