##Aspose::Cells::LowCode::AbstractLowCodeLoadOptionsProvider class
'Aspose::Cells::LowCode::AbstractLowCodeLoadOptionsProvider class. Implementation to provide multiple load options for processes that use multiple inputs(such as template files) in C++.'
## AbstractLowCodeLoadOptionsProvider class
Implementation to provide multiple load options for processes that use multiple inputs(such as template files).
```cpp
class AbstractLowCodeLoadOptionsProvider
```
## Methods
| Method | Description |
| --- | --- |
| [AbstractLowCodeLoadOptionsProvider(AbstractLowCodeLoadOptionsProvider_Impl* impl)](./abstractlowcodeloadoptionsprovider/) | Constructs from an implementation object. |
| [AbstractLowCodeLoadOptionsProvider(const AbstractLowCodeLoadOptionsProvider\& src)](./abstractlowcodeloadoptionsprovider/) | Copy constructor. |
| [Finish(const LowCodeLoadOptions\& part)](./finish/) | Releases resources after processing currently part of input. |
| virtual [GetCurrent()](./getcurrent/) | Gets the load options from which to load data of currently processed part. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| virtual [MoveNext()](./movenext/) | Checks whether there is more input. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const AbstractLowCodeLoadOptionsProvider\& src)](./operator_asm/) | operator= |
| [~AbstractLowCodeLoadOptionsProvider()](./~abstractlowcodeloadoptionsprovider/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Remarks
For example, [SpreadsheetMerger](../spreadsheetmerger/) feature requires multiple template files to merge.
## See Also
* Namespace [Aspose::Cells::LowCode](../)
* Library [Aspose.Cells for C++](../../)
