##Aspose::Cells::LowCode::SpreadsheetConverter class
'Aspose::Cells::LowCode::SpreadsheetConverter class. Converter for conversion between different spreadsheet file formats, such as xls, xlsx, xlsb, spreadsheet ml in C++.'
## SpreadsheetConverter class
Converter for conversion between different spreadsheet file formats, such as xls, xlsx, xlsb, spreadsheet ml...
```cpp
class SpreadsheetConverter
```
## Methods
| Method | Description |
| --- | --- |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SpreadsheetConverter\& src)](./operator_asm/) | operator= |
| static [Process(const U16String\& templateFile, const U16String\& resultFile)](./process/) | Converts given template file between spreadsheet file formats. |
| static [Process(const char16_t* templateFile, const char16_t* resultFile)](./process/) | Converts given template file between spreadsheet file formats. |
| static [Process(const LowCodeLoadOptions\& loadOptions, const LowCodeSaveOptions\& saveOptions)](./process/) | Converts between different spreadsheet file formats. |
| [SpreadsheetConverter(SpreadsheetConverter_Impl* impl)](./spreadsheetconverter/) | Constructs from an implementation object. |
| [SpreadsheetConverter(const SpreadsheetConverter\& src)](./spreadsheetconverter/) | Copy constructor. |
| [~SpreadsheetConverter()](./~spreadsheetconverter/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
SpreadsheetConverter::Process(u"template.xlsx", u"template.xlsb");
```
## See Also
* Namespace [Aspose::Cells::LowCode](../)
* Library [Aspose.Cells for C++](../../)
