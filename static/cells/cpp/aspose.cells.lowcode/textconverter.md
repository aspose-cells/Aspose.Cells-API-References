##Aspose::Cells::LowCode::TextConverter class
'Aspose::Cells::LowCode::TextConverter class. Converter for conversion between text based formats(csv, tsv, dif...) and other spreadsheet file formats in C++.'
## TextConverter class
Converter for conversion between text based formats(csv, tsv, dif...) and other spreadsheet file formats.
```cpp
class TextConverter
```
## Methods
| Method | Description |
| --- | --- |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const TextConverter\& src)](./operator_asm/) | operator= |
| static [Process(const U16String\& templateFile, const U16String\& resultFile)](./process/) | Converts given template file between text based files and other formats. |
| static [Process(const char16_t* templateFile, const char16_t* resultFile)](./process/) | Converts given template file between text based files and other formats. |
| static [Process(const LowCodeLoadOptions\& loadOptions, const LowCodeSaveOptions\& saveOptions)](./process/) | Converts file format between text based formats and other spreadsheet file formats. |
| [TextConverter(TextConverter_Impl* impl)](./textconverter/) | Constructs from an implementation object. |
| [TextConverter(const TextConverter\& src)](./textconverter/) | Copy constructor. |
| [~TextConverter()](./~textconverter/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
TextConverter::Process(u"template.csv", u"res.xlsx");
```
## See Also
* Namespace [Aspose::Cells::LowCode](../)
* Library [Aspose.Cells for C++](../../)
