##Aspose::Cells::LowCode::SpreadsheetLocker class
'Aspose::Cells::LowCode::SpreadsheetLocker class. Low code api to lock spreadsheet file in C++.'
## SpreadsheetLocker class
Low code api to lock spreadsheet file.
```cpp
class SpreadsheetLocker
```
## Methods
| Method | Description |
| --- | --- |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SpreadsheetLocker\& src)](./operator_asm/) | operator= |
| static [Process(const U16String\& templateFile, const U16String\& resultFile, const U16String\& openPassword, const U16String\& writePassword)](./process/) | Locks spreadsheet file with specified settings. |
| static [Process(const char16_t* templateFile, const char16_t* resultFile, const char16_t* openPassword, const char16_t* writePassword)](./process/) | Locks spreadsheet file with specified settings. |
| static [Process(const LowCodeLoadOptions\& loadOptions, const LowCodeSaveOptions\& saveOptions, const U16String\& openPassword, const U16String\& writePassword)](./process/) | Locks spreadsheet file with specified settings. |
| static [Process(const LowCodeLoadOptions\& loadOptions, const LowCodeSaveOptions\& saveOptions, const char16_t* openPassword, const char16_t* writePassword)](./process/) | Locks spreadsheet file with specified settings. |
| static [Process(const LowCodeLoadOptions\& loadOptions, const LowCodeSaveOptions\& saveOptions, const U16String\& openPassword, const U16String\& writePassword, const U16String\& workbookPassword, ProtectionType workbookType)](./process/) | Locks spreadsheet file with specified settings. |
| static [Process(const LowCodeLoadOptions\& loadOptions, const LowCodeSaveOptions\& saveOptions, const char16_t* openPassword, const char16_t* writePassword, const char16_t* workbookPassword, ProtectionType workbookType)](./process/) | Locks spreadsheet file with specified settings. |
| static [Process(const LowCodeLoadOptions\& loadOptions, const LowCodeSaveOptions\& saveOptions, const AbstractLowCodeProtectionProvider\& provider)](./process/) | Locks spreadsheet file with specified settings. |
| [SpreadsheetLocker(SpreadsheetLocker_Impl* impl)](./spreadsheetlocker/) | Constructs from an implementation object. |
| [SpreadsheetLocker(const SpreadsheetLocker\& src)](./spreadsheetlocker/) | Copy constructor. |
| [~SpreadsheetLocker()](./~spreadsheetlocker/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
SpreadsheetLocker::Process(u"template.xlsx", u"locked.xlsx", u"mypassword", u"mypassword");
```
## See Also
* Namespace [Aspose::Cells::LowCode](../)
* Library [Aspose.Cells for C++](../../)
