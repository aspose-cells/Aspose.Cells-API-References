##Aspose::Cells::LowCode::LowCodeSaveOptionsProviderOfAssembling class
'Aspose::Cells::LowCode::LowCodeSaveOptionsProviderOfAssembling class. Implementation to provide save options which save split parts to files and the path of resultant file are named as(it may contains directories): PathHeader+SheetPrefix+SheetIndex(or SheetName) +SplitPartPrefix+SplitPartIndex+PathTail in C++.'
## LowCodeSaveOptionsProviderOfAssembling class
Implementation to provide save options which save split parts to files and the path of resultant file are named as(it may contains directories): PathHeader+SheetPrefix+SheetIndex(or SheetName) +SplitPartPrefix+SplitPartIndex+PathTail.
```cpp
class LowCodeSaveOptionsProviderOfAssembling : public Aspose::Cells::LowCode::AbstractLowCodeSaveOptionsProvider
```
## Methods
| Method | Description |
| --- | --- |
| [AbstractLowCodeSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider_Impl* impl)](../abstractlowcodesaveoptionsprovider/abstractlowcodesaveoptionsprovider/) | Constructs from an implementation object. |
| [AbstractLowCodeSaveOptionsProvider(const AbstractLowCodeSaveOptionsProvider\& src)](../abstractlowcodesaveoptionsprovider/abstractlowcodesaveoptionsprovider/) | Copy constructor. |
| [Finish(const LowCodeSaveOptions\& part)](../abstractlowcodesaveoptionsprovider/finish/) | Releases resources after processing currently split part. |
| [GetBuildPathWithSheetAlways()](./getbuildpathwithsheetalways/) | Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index(or name) and corresponding prefix will not be added to the file path. |
| [GetBuildPathWithSplitPartAlways()](./getbuildpathwithsplitpartalways/) | Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix will not be added to the file path. |
| [GetPathHeader()](./getpathheader/) | Header part(before added content of sheet and split part) of file path. |
| [GetPathTail()](./getpathtail/) | Tailing part(after sequence numbers) of file path. It should include extension of file name. |
| virtual [GetSaveOptions(const SplitPartInfo\& part)](./getsaveoptions/) | Gets the save options from which to get the output settings for currently split part. |
| [GetSaveOptionsTemplate()](./getsaveoptionstemplate/) | The template for creating instance of save options in GetSaveOptions(SplitPartInfo). |
| [GetSheetIndexOffset()](./getsheetindexoffset/) | Offset of sheet's index between what used in file path and its actual value(SplitPartInfo.SheetIndex). |
| [GetSheetPrefix()](./getsheetprefix/) | Prefix for the index of worksheet. |
| [GetSplitPartIndexOffset()](./getsplitpartindexoffset/) | Offset of split part's index between what used in file path and its actual value(SplitPartInfo.PartIndex). |
| [GetSplitPartPrefix()](./getsplitpartprefix/) | Prefix for the index of split part. |
| [GetUseSheetName()](./getusesheetname/) | Whether builds the file path with sheet name instead of sheet index. Default value is false. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [LowCodeSaveOptionsProviderOfAssembling()](./lowcodesaveoptionsproviderofassembling/) | Default constructor. |
| [LowCodeSaveOptionsProviderOfAssembling(LowCodeSaveOptionsProviderOfAssembling_Impl* impl)](./lowcodesaveoptionsproviderofassembling/) | Constructs from an implementation object. |
| [LowCodeSaveOptionsProviderOfAssembling(const LowCodeSaveOptionsProviderOfAssembling\& src)](./lowcodesaveoptionsproviderofassembling/) | Copy constructor. |
| [LowCodeSaveOptionsProviderOfAssembling(const AbstractLowCodeSaveOptionsProvider\& src)](./lowcodesaveoptionsproviderofassembling/) | Constructs from a parent object. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const LowCodeSaveOptionsProviderOfAssembling\& src)](./operator_asm/) | operator= |
| [operator=(const AbstractLowCodeSaveOptionsProvider\& src)](../abstractlowcodesaveoptionsprovider/operator_asm/) | operator= |
| [SetBuildPathWithSheetAlways(bool value)](./setbuildpathwithsheetalways/) | Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index(or name) and corresponding prefix will not be added to the file path. |
| [SetBuildPathWithSplitPartAlways(bool value)](./setbuildpathwithsplitpartalways/) | Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix will not be added to the file path. |
| [SetPathHeader(const U16String\& value)](./setpathheader/) | Header part(before added content of sheet and split part) of file path. |
| [SetPathHeader(const char16_t* value)](./setpathheader/) | Header part(before added content of sheet and split part) of file path. |
| [SetPathTail(const U16String\& value)](./setpathtail/) | Tailing part(after sequence numbers) of file path. It should include extension of file name. |
| [SetPathTail(const char16_t* value)](./setpathtail/) | Tailing part(after sequence numbers) of file path. It should include extension of file name. |
| [SetSaveOptionsTemplate(const LowCodeSaveOptions\& value)](./setsaveoptionstemplate/) | The template for creating instance of save options in GetSaveOptions(SplitPartInfo). |
| [SetSheetIndexOffset(int32_t value)](./setsheetindexoffset/) | Offset of sheet's index between what used in file path and its actual value(SplitPartInfo.SheetIndex). |
| [SetSheetPrefix(const U16String\& value)](./setsheetprefix/) | Prefix for the index of worksheet. |
| [SetSheetPrefix(const char16_t* value)](./setsheetprefix/) | Prefix for the index of worksheet. |
| [SetSplitPartIndexOffset(int32_t value)](./setsplitpartindexoffset/) | Offset of split part's index between what used in file path and its actual value(SplitPartInfo.PartIndex). |
| [SetSplitPartPrefix(const U16String\& value)](./setsplitpartprefix/) | Prefix for the index of split part. |
| [SetSplitPartPrefix(const char16_t* value)](./setsplitpartprefix/) | Prefix for the index of split part. |
| [SetUseSheetName(bool value)](./setusesheetname/) | Whether builds the file path with sheet name instead of sheet index. Default value is false. |
| [~AbstractLowCodeSaveOptionsProvider()](../abstractlowcodesaveoptionsprovider/~abstractlowcodesaveoptionsprovider/) | Destructor. |
| [~LowCodeSaveOptionsProviderOfAssembling()](./~lowcodesaveoptionsproviderofassembling/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* Namespace [Aspose::Cells::LowCode](../)
* Library [Aspose.Cells for C++](../../)
