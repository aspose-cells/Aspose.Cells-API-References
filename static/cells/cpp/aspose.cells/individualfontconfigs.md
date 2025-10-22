##Aspose::Cells::IndividualFontConfigs class
'Aspose::Cells::IndividualFontConfigs class. Font configs for each Workbook object in C++.'
## IndividualFontConfigs class
[Font](../font/) configs for each [Workbook](../workbook/) object.
```cpp
class IndividualFontConfigs
```
## Methods
| Method | Description |
| --- | --- |
| [GetFontSources()](./getfontsources/) | Gets a copy of the array that contains the list of sources. |
| [GetFontSubstitutes(const U16String\& originalFontName)](./getfontsubstitutes/) | Returns array containing font substitute names to be used if original font is not presented. |
| [GetFontSubstitutes(const char16_t* originalFontName)](./getfontsubstitutes/) | Returns array containing font substitute names to be used if original font is not presented. |
| [IndividualFontConfigs()](./individualfontconfigs/) | Ctor. |
| [IndividualFontConfigs(IndividualFontConfigs_Impl* impl)](./individualfontconfigs/) | Constructs from an implementation object. |
| [IndividualFontConfigs(const IndividualFontConfigs\& src)](./individualfontconfigs/) | Copy constructor. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const IndividualFontConfigs\& src)](./operator_asm/) | operator= |
| [SetFontFolder(const U16String\& fontFolder, bool recursive)](./setfontfolder/) | Sets the fonts folder. |
| [SetFontFolder(const char16_t* fontFolder, bool recursive)](./setfontfolder/) | Sets the fonts folder. |
| [SetFontFolders(const Vector \<U16String\>\& fontFolders, bool recursive)](./setfontfolders/) | Sets the fonts folders. |
| [SetFontSources(const Vector \<FontSourceBase\>\& sources)](./setfontsources/) | Sets the fonts sources. |
| [SetFontSubstitutes(const U16String\& originalFontName, const Vector \<U16String\>\& substituteFontNames)](./setfontsubstitutes/) | [Font](../font/) substitute names for given original font name. |
| [SetFontSubstitutes(const char16_t* originalFontName, const Vector \<U16String\>\& substituteFontNames)](./setfontsubstitutes/) | [Font](../font/) substitute names for given original font name. |
| [~IndividualFontConfigs()](./~individualfontconfigs/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
