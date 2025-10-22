##Aspose::Cells::LowCode::JsonConverter class
'Aspose::Cells::LowCode::JsonConverter class. Converter for conversion between json data structure and other spreadsheet file formats in C++.'
## JsonConverter class
Converter for conversion between json data structure and other spreadsheet file formats.
```cpp
class JsonConverter
```
## Methods
| Method | Description |
| --- | --- |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [JsonConverter(JsonConverter_Impl* impl)](./jsonconverter/) | Constructs from an implementation object. |
| [JsonConverter(const JsonConverter\& src)](./jsonconverter/) | Copy constructor. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const JsonConverter\& src)](./operator_asm/) | operator= |
| static [Process(const U16String\& templateFile, const U16String\& resultFile)](./process/) | Converts given template file between json and other formats. |
| static [Process(const char16_t* templateFile, const char16_t* resultFile)](./process/) | Converts given template file between json and other formats. |
| static [Process(const LowCodeLoadOptions\& loadOptions, const LowCodeSaveOptions\& saveOptions)](./process/) | Converts between json data and other spreadsheet file formats. |
| [~JsonConverter()](./~jsonconverter/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
JsonConverter::Process(u"data.json", u"res.xlsx");
```
## See Also
* Namespace [Aspose::Cells::LowCode](../)
* Library [Aspose.Cells for C++](../../)
