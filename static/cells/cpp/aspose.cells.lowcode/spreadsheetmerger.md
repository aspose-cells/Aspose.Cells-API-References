##Aspose::Cells::LowCode::SpreadsheetMerger class
'Aspose::Cells::LowCode::SpreadsheetMerger class. Merges multiple template files into one in C++.'
## SpreadsheetMerger class
Merges multiple template files into one.
```cpp
class SpreadsheetMerger
```
## Methods
| Method | Description |
| --- | --- |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SpreadsheetMerger\& src)](./operator_asm/) | operator= |
| static [Process(const Vector \<U16String\>\& templateFiles, const U16String\& resultFile)](./process/) | Merge given template files. |
| static [Process(const Vector \<U16String\>\& templateFiles, const char16_t* resultFile)](./process/) | Merge given template files. |
| static [Process(const LowCodeMergeOptions\& options)](./process/) | Merges multiple template files into one. |
| [SpreadsheetMerger(SpreadsheetMerger_Impl* impl)](./spreadsheetmerger/) | Constructs from an implementation object. |
| [SpreadsheetMerger(const SpreadsheetMerger\& src)](./spreadsheetmerger/) | Copy constructor. |
| [~SpreadsheetMerger()](./~spreadsheetmerger/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
SpreadsheetMerger::Process(Vector<U16String>{ u"template2.xlsx", u"template2.xlsx", }, u"res.xlsx");
```
## See Also
* Namespace [Aspose::Cells::LowCode](../)
* Library [Aspose.Cells for C++](../../)
