##Aspose::Cells::LowCode::SpreadsheetSplitter::Process method
'Aspose::Cells::LowCode::SpreadsheetSplitter::Process method. Splits given template file into multiple parts in C++.'
## SpreadsheetSplitter::Process(const U16String\&, const U16String\&) method
Splits given template file into multiple parts.
```cpp
static void Aspose::Cells::LowCode::SpreadsheetSplitter::Process(const U16String &templateFile, const U16String &resultFile)
```
| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | const U16String\& | The template file to be split |
| resultFile | const U16String\& | The resultant file(name pattern) |
## Remarks
The output files will be build from the specified resultant file by appending sequence number of the sheet and split part. For example, if the specified output file is Split.xlsx, then the generated files will be Split_0_0.xlsx, Split_0_1.xlsx, ..., Split_1_0.xlsx, ...
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [SpreadsheetSplitter](../)
* Namespace [Aspose::Cells::LowCode](../../)
* Library [Aspose.Cells for C++](../../../)
## SpreadsheetSplitter::Process(const char16_t*, const char16_t*) method
Splits given template file into multiple parts.
```cpp
static void Aspose::Cells::LowCode::SpreadsheetSplitter::Process(const char16_t *templateFile, const char16_t *resultFile)
```
| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | const char16_t* | The template file to be split |
| resultFile | const char16_t* | The resultant file(name pattern) |
## Remarks
The output files will be build from the specified resultant file by appending sequence number of the sheet and split part. For example, if the specified output file is Split.xlsx, then the generated files will be Split_0_0.xlsx, Split_0_1.xlsx, ..., Split_1_0.xlsx, ...
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [SpreadsheetSplitter](../)
* Namespace [Aspose::Cells::LowCode](../../)
* Library [Aspose.Cells for C++](../../../)
## SpreadsheetSplitter::Process(const LowCodeSplitOptions\&) method
Splits spreadsheet file into multiple parts.
```cpp
static void Aspose::Cells::LowCode::SpreadsheetSplitter::Process(const LowCodeSplitOptions &options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| options | const LowCodeSplitOptions\& | Options for splitting spreadsheet |
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [LowCodeSplitOptions](../../lowcodesplitoptions/)
* Class [SpreadsheetSplitter](../)
* Namespace [Aspose::Cells::LowCode](../../)
* Library [Aspose.Cells for C++](../../../)
