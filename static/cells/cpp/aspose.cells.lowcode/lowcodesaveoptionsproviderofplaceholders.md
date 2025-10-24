##Aspose::Cells::LowCode::LowCodeSaveOptionsProviderOfPlaceHolders class
'Aspose::Cells::LowCode::LowCodeSaveOptionsProviderOfPlaceHolders class. Implementation to provide save options which save split parts to files and the path of resultant file are defined with placeholders in C++.'
## LowCodeSaveOptionsProviderOfPlaceHolders class
Implementation to provide save options which save split parts to files and the path of resultant file are defined with placeholders.
```cpp
class LowCodeSaveOptionsProviderOfPlaceHolders : public Aspose::Cells::LowCode::AbstractLowCodeSaveOptionsProvider
```
## Methods
| Method | Description |
| --- | --- |
| [AbstractLowCodeSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider_Impl* impl)](../abstractlowcodesaveoptionsprovider/abstractlowcodesaveoptionsprovider/) | Constructs from an implementation object. |
| [AbstractLowCodeSaveOptionsProvider(const AbstractLowCodeSaveOptionsProvider\& src)](../abstractlowcodesaveoptionsprovider/abstractlowcodesaveoptionsprovider/) | Copy constructor. |
| [Finish(const LowCodeSaveOptions\& part)](../abstractlowcodesaveoptionsprovider/finish/) | Releases resources after processing currently split part. |
| [GetBuildPathWithSheetAlways()](./getbuildpathwithsheetalways/) | Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index and name and corresponding prefix(SheetNamePrefix) will not be added to the file path. |
| [GetBuildPathWithSplitPartAlways()](./getbuildpathwithsplitpartalways/) | Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix(SplitPartPrefix) will not be added to the file path. |
| virtual [GetSaveOptions(const SplitPartInfo\& part)](./getsaveoptions/) | Gets the save options from which to get the output settings for currently split part. |
| [GetSaveOptionsTemplate()](./getsaveoptionstemplate/) | The template for creating instance of save options in GetSaveOptions(SplitPartInfo). |
| [GetSheetIndexOffset()](./getsheetindexoffset/) | Offset of sheet's index between what used in file path and its actual value(SplitPartInfo.SheetIndex). |
| [GetSheetIndexPrefix()](./getsheetindexprefix/) | Prefix for the index of worksheet. |
| [GetSheetNamePrefix()](./getsheetnameprefix/) | Prefix for the index of worksheet. |
| [GetSplitPartIndexOffset()](./getsplitpartindexoffset/) | Offset of split part's index between what used in file path and its actual value(SplitPartInfo.PartIndex). |
| [GetSplitPartPrefix()](./getsplitpartprefix/) | Prefix for the index of split part. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [LowCodeSaveOptionsProviderOfPlaceHolders(const U16String\& pathTemplate)](./lowcodesaveoptionsproviderofplaceholders/) | Instantiates an instance to provide save options according to specified templates. |
| explicit [LowCodeSaveOptionsProviderOfPlaceHolders(const char16_t* pathTemplate)](./lowcodesaveoptionsproviderofplaceholders/) | Instantiates an instance to provide save options according to specified templates. |
| [LowCodeSaveOptionsProviderOfPlaceHolders(LowCodeSaveOptionsProviderOfPlaceHolders_Impl* impl)](./lowcodesaveoptionsproviderofplaceholders/) | Constructs from an implementation object. |
| [LowCodeSaveOptionsProviderOfPlaceHolders(const LowCodeSaveOptionsProviderOfPlaceHolders\& src)](./lowcodesaveoptionsproviderofplaceholders/) | Copy constructor. |
| [LowCodeSaveOptionsProviderOfPlaceHolders(const AbstractLowCodeSaveOptionsProvider\& src)](./lowcodesaveoptionsproviderofplaceholders/) | Constructs from a parent object. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const LowCodeSaveOptionsProviderOfPlaceHolders\& src)](./operator_asm/) | operator= |
| [operator=(const AbstractLowCodeSaveOptionsProvider\& src)](../abstractlowcodesaveoptionsprovider/operator_asm/) | operator= |
| [SetBuildPathWithSheetAlways(bool value)](./setbuildpathwithsheetalways/) | Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index and name and corresponding prefix(SheetNamePrefix) will not be added to the file path. |
| [SetBuildPathWithSplitPartAlways(bool value)](./setbuildpathwithsplitpartalways/) | Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix(SplitPartPrefix) will not be added to the file path. |
| [SetSaveOptionsTemplate(const LowCodeSaveOptions\& value)](./setsaveoptionstemplate/) | The template for creating instance of save options in GetSaveOptions(SplitPartInfo). |
| [SetSheetIndexOffset(int32_t value)](./setsheetindexoffset/) | Offset of sheet's index between what used in file path and its actual value(SplitPartInfo.SheetIndex). |
| [SetSheetIndexPrefix(const U16String\& value)](./setsheetindexprefix/) | Prefix for the index of worksheet. |
| [SetSheetIndexPrefix(const char16_t* value)](./setsheetindexprefix/) | Prefix for the index of worksheet. |
| [SetSheetNamePrefix(const U16String\& value)](./setsheetnameprefix/) | Prefix for the index of worksheet. |
| [SetSheetNamePrefix(const char16_t* value)](./setsheetnameprefix/) | Prefix for the index of worksheet. |
| [SetSplitPartIndexOffset(int32_t value)](./setsplitpartindexoffset/) | Offset of split part's index between what used in file path and its actual value(SplitPartInfo.PartIndex). |
| [SetSplitPartPrefix(const U16String\& value)](./setsplitpartprefix/) | Prefix for the index of split part. |
| [SetSplitPartPrefix(const char16_t* value)](./setsplitpartprefix/) | Prefix for the index of split part. |
| [~AbstractLowCodeSaveOptionsProvider()](../abstractlowcodesaveoptionsprovider/~abstractlowcodesaveoptionsprovider/) | Destructor. |
| [~LowCodeSaveOptionsProviderOfPlaceHolders()](./~lowcodesaveoptionsproviderofplaceholders/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* Namespace [Aspose::Cells::LowCode](../)
* Library [Aspose.Cells for C++](../../)
