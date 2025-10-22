##Aspose::Cells::LowCode::SplitPartInfo class
'Aspose::Cells::LowCode::SplitPartInfo class. Represents the information of one input/output for multiple inputs/outputs, such as current page to be rendered when converting spreadsheet to image in C++.'
## SplitPartInfo class
Represents the information of one input/output for multiple inputs/outputs, such as current page to be rendered when converting spreadsheet to image.
```cpp
class SplitPartInfo
```
## Methods
| Method | Description |
| --- | --- |
| [GetPartIndex()](./getpartindex/) | Index of current part in sequence(0 based). -1 means there are no multiple parts so the result is single. |
| [GetSheetIndex()](./getsheetindex/) | Index of the sheet where current part is in. -1 denotes there is only one sheet. |
| [GetSheetName()](./getsheetname/) | [Name](../../aspose.cells/name/) of the sheet where current part is in. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SplitPartInfo\& src)](./operator_asm/) | operator= |
| [SplitPartInfo(SplitPartInfo_Impl* impl)](./splitpartinfo/) | Constructs from an implementation object. |
| [SplitPartInfo(const SplitPartInfo\& src)](./splitpartinfo/) | Copy constructor. |
| [~SplitPartInfo()](./~splitpartinfo/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells::LowCode](../)
* Library [Aspose.Cells for C++](../../)
