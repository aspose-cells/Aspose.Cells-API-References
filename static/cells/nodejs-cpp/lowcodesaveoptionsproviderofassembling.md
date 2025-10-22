##LowCodeSaveOptionsProviderOfAssembling
Implementation to provide save options which save split parts to files and the path of resultant file are named asit may contains directories PathHeader..pathheaderSheetPrefix..sheetprefixSheetIndexor SheetName SplitPartPrefix..splitpartprefixSplitPartIndexPathTail..pathtail.
## LowCodeSaveOptionsProviderOfAssembling class
Implementation to provide save options which save split parts to files and the path of resultant file are named as(it may contains directories): [PathHeader](../pathheader/)+[SheetPrefix](../sheetprefix/)+SheetIndex(or SheetName) +[SplitPartPrefix](../splitpartprefix/)+SplitPartIndex+[PathTail](../pathtail/).
```javascript
class LowCodeSaveOptionsProviderOfAssembling extends AbstractLowCodeSaveOptionsProvider;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(AbstractLowCodeSaveOptionsProvider)](#constructor-abstractlowcodesaveoptionsprovider-)| Constructs from a parent object convertible to this. |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [pathHeader](#pathHeader--)| string | Header part(before added content of sheet and split part) of file path. |
| [pathTail](#pathTail--)| string | Tailing part(after sequence numbers) of file path. It should include extension of file name. |
| [useSheetName](#useSheetName--)| boolean | Whether builds the file path with sheet name instead of sheet index. Default value is false. |
| [sheetPrefix](#sheetPrefix--)| string | Prefix for the index of worksheet. |
| [splitPartPrefix](#splitPartPrefix--)| string | Prefix for the index of split part. |
| [sheetIndexOffset](#sheetIndexOffset--)| number | Offset of sheet's index between what used in file path and its actual value([SplitPartInfo.SheetIndex](../splitpartinfo.sheetindex/)). |
| [splitPartIndexOffset](#splitPartIndexOffset--)| number | Offset of split part's index between what used in file path and its actual value([SplitPartInfo.PartIndex](../splitpartinfo.partindex/)). |
| [buildPathWithSheetAlways](#buildPathWithSheetAlways--)| boolean | Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index(or name) and corresponding prefix will not be added to the file path. |
| [buildPathWithSplitPartAlways](#buildPathWithSplitPartAlways--)| boolean | Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix will not be added to the file path. |
| [saveOptionsTemplate](#saveOptionsTemplate--)| LowCodeSaveOptions | The template for creating instance of save options in [GetSaveOptions(SplitPartInfo)](../getsaveoptions(splitpartinfo)/). |
## Methods
| Method | Description |
| --- | --- |
| [getPathHeader()](#getPathHeader--)| <b>@deprecated.</b> Please use the 'pathHeader' property instead. Header part(before added content of sheet and split part) of file path. |
| [setPathHeader(string)](#setPathHeader-string-)| <b>@deprecated.</b> Please use the 'pathHeader' property instead. Header part(before added content of sheet and split part) of file path. |
| [getPathTail()](#getPathTail--)| <b>@deprecated.</b> Please use the 'pathTail' property instead. Tailing part(after sequence numbers) of file path. It should include extension of file name. |
| [setPathTail(string)](#setPathTail-string-)| <b>@deprecated.</b> Please use the 'pathTail' property instead. Tailing part(after sequence numbers) of file path. It should include extension of file name. |
| [getUseSheetName()](#getUseSheetName--)| <b>@deprecated.</b> Please use the 'useSheetName' property instead. Whether builds the file path with sheet name instead of sheet index. Default value is false. |
| [setUseSheetName(boolean)](#setUseSheetName-boolean-)| <b>@deprecated.</b> Please use the 'useSheetName' property instead. Whether builds the file path with sheet name instead of sheet index. Default value is false. |
| [getSheetPrefix()](#getSheetPrefix--)| <b>@deprecated.</b> Please use the 'sheetPrefix' property instead. Prefix for the index of worksheet. |
| [setSheetPrefix(string)](#setSheetPrefix-string-)| <b>@deprecated.</b> Please use the 'sheetPrefix' property instead. Prefix for the index of worksheet. |
| [getSplitPartPrefix()](#getSplitPartPrefix--)| <b>@deprecated.</b> Please use the 'splitPartPrefix' property instead. Prefix for the index of split part. |
| [setSplitPartPrefix(string)](#setSplitPartPrefix-string-)| <b>@deprecated.</b> Please use the 'splitPartPrefix' property instead. Prefix for the index of split part. |
| [getSheetIndexOffset()](#getSheetIndexOffset--)| <b>@deprecated.</b> Please use the 'sheetIndexOffset' property instead. Offset of sheet's index between what used in file path and its actual value([SplitPartInfo.SheetIndex](../splitpartinfo.sheetindex/)). |
| [setSheetIndexOffset(number)](#setSheetIndexOffset-number-)| <b>@deprecated.</b> Please use the 'sheetIndexOffset' property instead. Offset of sheet's index between what used in file path and its actual value([SplitPartInfo.SheetIndex](../splitpartinfo.sheetindex/)). |
| [getSplitPartIndexOffset()](#getSplitPartIndexOffset--)| <b>@deprecated.</b> Please use the 'splitPartIndexOffset' property instead. Offset of split part's index between what used in file path and its actual value([SplitPartInfo.PartIndex](../splitpartinfo.partindex/)). |
| [setSplitPartIndexOffset(number)](#setSplitPartIndexOffset-number-)| <b>@deprecated.</b> Please use the 'splitPartIndexOffset' property instead. Offset of split part's index between what used in file path and its actual value([SplitPartInfo.PartIndex](../splitpartinfo.partindex/)). |
| [getBuildPathWithSheetAlways()](#getBuildPathWithSheetAlways--)| <b>@deprecated.</b> Please use the 'buildPathWithSheetAlways' property instead. Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index(or name) and corresponding prefix will not be added to the file path. |
| [setBuildPathWithSheetAlways(boolean)](#setBuildPathWithSheetAlways-boolean-)| <b>@deprecated.</b> Please use the 'buildPathWithSheetAlways' property instead. Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index(or name) and corresponding prefix will not be added to the file path. |
| [getBuildPathWithSplitPartAlways()](#getBuildPathWithSplitPartAlways--)| <b>@deprecated.</b> Please use the 'buildPathWithSplitPartAlways' property instead. Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix will not be added to the file path. |
| [setBuildPathWithSplitPartAlways(boolean)](#setBuildPathWithSplitPartAlways-boolean-)| <b>@deprecated.</b> Please use the 'buildPathWithSplitPartAlways' property instead. Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix will not be added to the file path. |
| [getSaveOptionsTemplate()](#getSaveOptionsTemplate--)| <b>@deprecated.</b> Please use the 'saveOptionsTemplate' property instead. The template for creating instance of save options in [GetSaveOptions(SplitPartInfo)](../getsaveoptions(splitpartinfo)/). |
| [setSaveOptionsTemplate(LowCodeSaveOptions)](#setSaveOptionsTemplate-lowcodesaveoptions-)| <b>@deprecated.</b> Please use the 'saveOptionsTemplate' property instead. The template for creating instance of save options in [GetSaveOptions(SplitPartInfo)](../getsaveoptions(splitpartinfo)/). |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getSaveOptions(SplitPartInfo)](#getSaveOptions-splitpartinfo-)| Gets the save options from which to get the output settings for currently split part. |
| [finish(LowCodeSaveOptions)](#finish-lowcodesaveoptions-)| Releases resources after processing currently split part. |
### constructor(AbstractLowCodeSaveOptionsProvider) {#constructor-abstractlowcodesaveoptionsprovider-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: AbstractLowCodeSaveOptionsProvider);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | AbstractLowCodeSaveOptionsProvider | The parent object. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### pathHeader {#pathHeader--}
Header part(before added content of sheet and split part) of file path.
```javascript
pathHeader : string;
```
### pathTail {#pathTail--}
Tailing part(after sequence numbers) of file path. It should include extension of file name.
```javascript
pathTail : string;
```
### useSheetName {#useSheetName--}
Whether builds the file path with sheet name instead of sheet index. Default value is false.
```javascript
useSheetName : boolean;
```
**Remarks**
The sheet name will never be rebuilt automatically. So when set it to true, please make sure there is no special sheet name that can cause invalid file path or name.
### sheetPrefix {#sheetPrefix--}
Prefix for the index of worksheet.
```javascript
sheetPrefix : string;
```
**Remarks**
If there is only one worksheet and [BuildPathWithSheetAlways](../buildpathwithsheetalways/) is false, then this prefix and the sheet index(or name) will not be added to the resultant file path.
### splitPartPrefix {#splitPartPrefix--}
Prefix for the index of split part.
```javascript
splitPartPrefix : string;
```
**Remarks**
If there is only one split part and [BuildPathWithSplitPartAlways](../buildpathwithsplitpartalways/) is false, then this prefix and the split part index(0) will not be added to the resultant file path.
### sheetIndexOffset {#sheetIndexOffset--}
Offset of sheet's index between what used in file path and its actual value([SplitPartInfo.SheetIndex](../splitpartinfo.sheetindex/)).
```javascript
sheetIndexOffset : number;
```
**Remarks**
Only takes effect when [UseSheetName](../usesheetname/) is false.
### splitPartIndexOffset {#splitPartIndexOffset--}
Offset of split part's index between what used in file path and its actual value([SplitPartInfo.PartIndex](../splitpartinfo.partindex/)).
```javascript
splitPartIndexOffset : number;
```
### buildPathWithSheetAlways {#buildPathWithSheetAlways--}
Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index(or name) and corresponding prefix will not be added to the file path.
```javascript
buildPathWithSheetAlways : boolean;
```
### buildPathWithSplitPartAlways {#buildPathWithSplitPartAlways--}
Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix will not be added to the file path.
```javascript
buildPathWithSplitPartAlways : boolean;
```
### saveOptionsTemplate {#saveOptionsTemplate--}
The template for creating instance of save options in [GetSaveOptions(SplitPartInfo)](../getsaveoptions(splitpartinfo)/).
```javascript
saveOptionsTemplate : LowCodeSaveOptions;
```
**Remarks**
If the template has been specified, then the created instance will copy all setting from it and update the output file accordingly.
### getPathHeader() {#getPathHeader--}
```javascript
getPathHeader() : string;
```
### setPathHeader(string) {#setPathHeader-string-}
```javascript
setPathHeader(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getPathTail() {#getPathTail--}
```javascript
getPathTail() : string;
```
### setPathTail(string) {#setPathTail-string-}
```javascript
setPathTail(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getUseSheetName() {#getUseSheetName--}
```javascript
getUseSheetName() : boolean;
```
**Remarks**
The sheet name will never be rebuilt automatically. So when set it to true, please make sure there is no special sheet name that can cause invalid file path or name.
### setUseSheetName(boolean) {#setUseSheetName-boolean-}
```javascript
setUseSheetName(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
The sheet name will never be rebuilt automatically. So when set it to true, please make sure there is no special sheet name that can cause invalid file path or name.
### getSheetPrefix() {#getSheetPrefix--}
```javascript
getSheetPrefix() : string;
```
**Remarks**
If there is only one worksheet and [BuildPathWithSheetAlways](../buildpathwithsheetalways/) is false, then this prefix and the sheet index(or name) will not be added to the resultant file path.
### setSheetPrefix(string) {#setSheetPrefix-string-}
```javascript
setSheetPrefix(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
If there is only one worksheet and [BuildPathWithSheetAlways](../buildpathwithsheetalways/) is false, then this prefix and the sheet index(or name) will not be added to the resultant file path.
### getSplitPartPrefix() {#getSplitPartPrefix--}
```javascript
getSplitPartPrefix() : string;
```
**Remarks**
If there is only one split part and [BuildPathWithSplitPartAlways](../buildpathwithsplitpartalways/) is false, then this prefix and the split part index(0) will not be added to the resultant file path.
### setSplitPartPrefix(string) {#setSplitPartPrefix-string-}
```javascript
setSplitPartPrefix(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
If there is only one split part and [BuildPathWithSplitPartAlways](../buildpathwithsplitpartalways/) is false, then this prefix and the split part index(0) will not be added to the resultant file path.
### getSheetIndexOffset() {#getSheetIndexOffset--}
```javascript
getSheetIndexOffset() : number;
```
**Remarks**
Only takes effect when [UseSheetName](../usesheetname/) is false.
### setSheetIndexOffset(number) {#setSheetIndexOffset-number-}
```javascript
setSheetIndexOffset(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
Only takes effect when [UseSheetName](../usesheetname/) is false.
### getSplitPartIndexOffset() {#getSplitPartIndexOffset--}
```javascript
getSplitPartIndexOffset() : number;
```
### setSplitPartIndexOffset(number) {#setSplitPartIndexOffset-number-}
```javascript
setSplitPartIndexOffset(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getBuildPathWithSheetAlways() {#getBuildPathWithSheetAlways--}
```javascript
getBuildPathWithSheetAlways() : boolean;
```
### setBuildPathWithSheetAlways(boolean) {#setBuildPathWithSheetAlways-boolean-}
```javascript
setBuildPathWithSheetAlways(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getBuildPathWithSplitPartAlways() {#getBuildPathWithSplitPartAlways--}
```javascript
getBuildPathWithSplitPartAlways() : boolean;
```
### setBuildPathWithSplitPartAlways(boolean) {#setBuildPathWithSplitPartAlways-boolean-}
```javascript
setBuildPathWithSplitPartAlways(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getSaveOptionsTemplate() {#getSaveOptionsTemplate--}
```javascript
getSaveOptionsTemplate() : LowCodeSaveOptions;
```
**Returns**
[LowCodeSaveOptions](../lowcodesaveoptions/)
**Remarks**
If the template has been specified, then the created instance will copy all setting from it and update the output file accordingly.
### setSaveOptionsTemplate(LowCodeSaveOptions) {#setSaveOptionsTemplate-lowcodesaveoptions-}
```javascript
setSaveOptionsTemplate(value: LowCodeSaveOptions) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LowCodeSaveOptions](../lowcodesaveoptions/) | The value to set. |
**Remarks**
If the template has been specified, then the created instance will copy all setting from it and update the output file accordingly.
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getSaveOptions(SplitPartInfo) {#getSaveOptions-splitpartinfo-}
Gets the save options from which to get the output settings for currently split part.
```javascript
getSaveOptions(part: SplitPartInfo) : LowCodeSaveOptions;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| part | [SplitPartInfo](../splitpartinfo/) |  |
**Returns**
[LowCodeSaveOptions](../lowcodesaveoptions/)
### finish(LowCodeSaveOptions) {#finish-lowcodesaveoptions-}
Releases resources after processing currently split part.
```javascript
finish(part: LowCodeSaveOptions) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| part | [LowCodeSaveOptions](../lowcodesaveoptions/) | the save options used for currently split part. |
**Remarks**
By default this method just closes the stream specified by the [LowCodeSaveOptions.OutputStream](../lowcodesaveoptions.outputstream/) directly(if the save options specified a Stream as destination). User may overwrite this method to control how to release resources according to their requirement and the implementation of [GetSaveOptions(SplitPartInfo)](../getsaveoptions(splitpartinfo)/).
