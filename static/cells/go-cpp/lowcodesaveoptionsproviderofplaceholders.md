##LowCodeSaveOptionsProviderOfPlaceHolders Class
'LowCodeSaveOptionsProviderOfPlaceHolders class. Encapsulates the object that represents lowcodesaveoptionsproviderofplaceholders in Go.'
## LowCodeSaveOptionsProviderOfPlaceHolders class
Implementation to provide save options which save split parts to filesand the path of resultant file are defined with placeholders.
```go
type LowCodeSaveOptionsProviderOfPlaceHolders struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewLowCodeSaveOptionsProviderOfPlaceHolders_String](./newlowcodesaveoptionsproviderofplaceholders_string/) | Instantiates an instance to provide save options according to specified templates. |
|[NewLowCodeSaveOptionsProviderOfPlaceHolders_AbstractLowCodeSaveOptionsProvider](./newlowcodesaveoptionsproviderofplaceholders_abstractlowcodesaveoptionsprovider/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetSheetIndexOffset](./getsheetindexoffset/) | Offset of sheet's index between what used in file pathand its actual value(SplitPartInfo.SheetIndex). |
|[SetSheetIndexOffset](./setsheetindexoffset/) | Offset of sheet's index between what used in file pathand its actual value(SplitPartInfo.SheetIndex). |
|[GetSplitPartIndexOffset](./getsplitpartindexoffset/) | Offset of split part's index between what used in file pathand its actual value(SplitPartInfo.PartIndex). |
|[SetSplitPartIndexOffset](./setsplitpartindexoffset/) | Offset of split part's index between what used in file pathand its actual value(SplitPartInfo.PartIndex). |
|[GetBuildPathWithSheetAlways](./getbuildpathwithsheetalways/) | Whether add sheet index or name to file path always.Default value is false, that is, when there is only one sheet,the sheet index and name and corresponding prefix(SheetNamePrefix)will not be added to the file path. |
|[SetBuildPathWithSheetAlways](./setbuildpathwithsheetalways/) | Whether add sheet index or name to file path always.Default value is false, that is, when there is only one sheet,the sheet index and name and corresponding prefix(SheetNamePrefix)will not be added to the file path. |
|[GetBuildPathWithSplitPartAlways](./getbuildpathwithsplitpartalways/) | Whether add split part index to file path always.Default value is false, that is, when there is only one split part,the split part index and corresponding prefix(SplitPartPrefix)will not be added to the file path. |
|[SetBuildPathWithSplitPartAlways](./setbuildpathwithsplitpartalways/) | Whether add split part index to file path always.Default value is false, that is, when there is only one split part,the split part index and corresponding prefix(SplitPartPrefix)will not be added to the file path. |
|[GetSheetNamePrefix](./getsheetnameprefix/) | Prefix for the index of worksheet. |
|[SetSheetNamePrefix](./setsheetnameprefix/) | Prefix for the index of worksheet. |
|[GetSheetIndexPrefix](./getsheetindexprefix/) | Prefix for the index of worksheet. |
|[SetSheetIndexPrefix](./setsheetindexprefix/) | Prefix for the index of worksheet. |
|[GetSplitPartPrefix](./getsplitpartprefix/) | Prefix for the index of split part. |
|[SetSplitPartPrefix](./setsplitpartprefix/) | Prefix for the index of split part. |
|[GetSaveOptionsTemplate](./getsaveoptionstemplate/) | The template for creating instance of save options in GetSaveOptions(SplitPartInfo). |
|[SetSaveOptionsTemplate](./setsaveoptionstemplate/) | The template for creating instance of save options in GetSaveOptions(SplitPartInfo). |
|[GetSaveOptions](./getsaveoptions/) | Gets the save options from which to get the output settings for currently split part. |
|[Finish](./finish/) | Releases resources after processing currently split part. |
