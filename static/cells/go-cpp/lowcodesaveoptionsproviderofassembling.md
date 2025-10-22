##LowCodeSaveOptionsProviderOfAssembling Class
'LowCodeSaveOptionsProviderOfAssembling class. Encapsulates the object that represents lowcodesaveoptionsproviderofassembling in Go.'
## LowCodeSaveOptionsProviderOfAssembling class
Implementation to provide save options which save split parts to filesand the path of resultant file are named as(it may contains directories):<see cref="PathHeader"/>+<see cref="SheetPrefix"/>+SheetIndex(or SheetName)+<see cref="SplitPartPrefix"/>+SplitPartIndex+<see cref="PathTail"/>.
```go
type LowCodeSaveOptionsProviderOfAssembling struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewLowCodeSaveOptionsProviderOfAssembling](./newlowcodesaveoptionsproviderofassembling/) | Default constructor. |
|[NewLowCodeSaveOptionsProviderOfAssembling_AbstractLowCodeSaveOptionsProvider](./newlowcodesaveoptionsproviderofassembling_abstractlowcodesaveoptionsprovider/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetPathHeader](./getpathheader/) | Header part(before added content of sheet and split part) of file path. |
|[SetPathHeader](./setpathheader/) | Header part(before added content of sheet and split part) of file path. |
|[GetPathTail](./getpathtail/) | Tailing part(after sequence numbers) of file path.It should include extension of file name. |
|[SetPathTail](./setpathtail/) | Tailing part(after sequence numbers) of file path.It should include extension of file name. |
|[GetUseSheetName](./getusesheetname/) | Whether builds the file path with sheet name instead of sheet index. Default value is false. |
|[SetUseSheetName](./setusesheetname/) | Whether builds the file path with sheet name instead of sheet index. Default value is false. |
|[GetSheetPrefix](./getsheetprefix/) | Prefix for the index of worksheet. |
|[SetSheetPrefix](./setsheetprefix/) | Prefix for the index of worksheet. |
|[GetSplitPartPrefix](./getsplitpartprefix/) | Prefix for the index of split part. |
|[SetSplitPartPrefix](./setsplitpartprefix/) | Prefix for the index of split part. |
|[GetSheetIndexOffset](./getsheetindexoffset/) | Offset of sheet's index between what used in file pathand its actual value(SplitPartInfo.SheetIndex). |
|[SetSheetIndexOffset](./setsheetindexoffset/) | Offset of sheet's index between what used in file pathand its actual value(SplitPartInfo.SheetIndex). |
|[GetSplitPartIndexOffset](./getsplitpartindexoffset/) | Offset of split part's index between what used in file pathand its actual value(SplitPartInfo.PartIndex). |
|[SetSplitPartIndexOffset](./setsplitpartindexoffset/) | Offset of split part's index between what used in file pathand its actual value(SplitPartInfo.PartIndex). |
|[GetBuildPathWithSheetAlways](./getbuildpathwithsheetalways/) | Whether add sheet index or name to file path always.Default value is false, that is, when there is only one sheet,the sheet index(or name) and corresponding prefix will not be added to the file path. |
|[SetBuildPathWithSheetAlways](./setbuildpathwithsheetalways/) | Whether add sheet index or name to file path always.Default value is false, that is, when there is only one sheet,the sheet index(or name) and corresponding prefix will not be added to the file path. |
|[GetBuildPathWithSplitPartAlways](./getbuildpathwithsplitpartalways/) | Whether add split part index to file path always.Default value is false, that is, when there is only one split part,the split part index and corresponding prefix will not be added to the file path. |
|[SetBuildPathWithSplitPartAlways](./setbuildpathwithsplitpartalways/) | Whether add split part index to file path always.Default value is false, that is, when there is only one split part,the split part index and corresponding prefix will not be added to the file path. |
|[GetSaveOptionsTemplate](./getsaveoptionstemplate/) | The template for creating instance of save options in GetSaveOptions(SplitPartInfo). |
|[SetSaveOptionsTemplate](./setsaveoptionstemplate/) | The template for creating instance of save options in GetSaveOptions(SplitPartInfo). |
|[GetSaveOptions](./getsaveoptions/) | Gets the save options from which to get the output settings for currently split part. |
|[Finish](./finish/) | Releases resources after processing currently split part. |
