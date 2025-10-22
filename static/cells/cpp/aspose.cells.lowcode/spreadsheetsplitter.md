##Aspose::Cells::LowCode::SpreadsheetSplitter class
'Aspose::Cells::LowCode::SpreadsheetSplitter class. Splits spreadsheet file into multiple parts in C++.'
## SpreadsheetSplitter class
Splits spreadsheet file into multiple parts.
```cpp
class SpreadsheetSplitter
```
## Methods
| Method | Description |
| --- | --- |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SpreadsheetSplitter\& src)](./operator_asm/) | operator= |
| static [Process(const U16String\& templateFile, const U16String\& resultFile)](./process/) | Splits given template file into multiple parts. |
| static [Process(const char16_t* templateFile, const char16_t* resultFile)](./process/) | Splits given template file into multiple parts. |
| static [Process(const LowCodeSplitOptions\& options)](./process/) | Splits spreadsheet file into multiple parts. |
| [SpreadsheetSplitter(SpreadsheetSplitter_Impl* impl)](./spreadsheetsplitter/) | Constructs from an implementation object. |
| [SpreadsheetSplitter(const SpreadsheetSplitter\& src)](./spreadsheetsplitter/) | Copy constructor. |
| [~SpreadsheetSplitter()](./~spreadsheetsplitter/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
SpreadsheetSplitter::Process(u"template.xlsx", u"split.xlsx");
```
## See Also
* Namespace [Aspose::Cells::LowCode](../)
* Library [Aspose.Cells for C++](../../)
