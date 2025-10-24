##Aspose::Cells::LowCode::AbstractLowCodeSaveOptionsProvider class
'Aspose::Cells::LowCode::AbstractLowCodeSaveOptionsProvider class. Implementation to provide multiple save options for processes that require multiple outputs. For example, SpreadsheetSplitter feature requires multiple destinations to save the split files in C++.'
## AbstractLowCodeSaveOptionsProvider class
Implementation to provide multiple save options for processes that require multiple outputs. For example, [SpreadsheetSplitter](../spreadsheetsplitter/) feature requires multiple destinations to save the split files.
```cpp
class AbstractLowCodeSaveOptionsProvider
```
## Methods
| Method | Description |
| --- | --- |
| [AbstractLowCodeSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider_Impl* impl)](./abstractlowcodesaveoptionsprovider/) | Constructs from an implementation object. |
| [AbstractLowCodeSaveOptionsProvider(const AbstractLowCodeSaveOptionsProvider\& src)](./abstractlowcodesaveoptionsprovider/) | Copy constructor. |
| [Finish(const LowCodeSaveOptions\& part)](./finish/) | Releases resources after processing currently split part. |
| virtual [GetSaveOptions(const SplitPartInfo\& part)](./getsaveoptions/) | Gets the save options from which to get the output settings for currently split part. Returning null denotes to skip given part. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const AbstractLowCodeSaveOptionsProvider\& src)](./operator_asm/) | operator= |
| [~AbstractLowCodeSaveOptionsProvider()](./~abstractlowcodesaveoptionsprovider/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells::LowCode](../)
* Library [Aspose.Cells for C++](../../)
