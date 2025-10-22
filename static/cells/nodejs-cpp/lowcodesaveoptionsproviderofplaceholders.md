##LowCodeSaveOptionsProviderOfPlaceHolders
Implementation to provide save options which save split parts to files and the path of resultant file are defined with placeholders.
## LowCodeSaveOptionsProviderOfPlaceHolders class
Implementation to provide save options which save split parts to files and the path of resultant file are defined with placeholders.
```javascript
class LowCodeSaveOptionsProviderOfPlaceHolders extends AbstractLowCodeSaveOptionsProvider;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(AbstractLowCodeSaveOptionsProvider)](#constructor-abstractlowcodesaveoptionsprovider-)| Constructs from a parent object convertible to this. |
| [constructor(string)](#constructor-string-)| Instantiates an instance to provide save options according to specified templates. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [sheetIndexOffset](#sheetIndexOffset--)| number | Offset of sheet's index between what used in file path and its actual value([SplitPartInfo.SheetIndex](../splitpartinfo.sheetindex/)). |
| [splitPartIndexOffset](#splitPartIndexOffset--)| number | Offset of split part's index between what used in file path and its actual value([SplitPartInfo.PartIndex](../splitpartinfo.partindex/)). |
| [buildPathWithSheetAlways](#buildPathWithSheetAlways--)| boolean | Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index and name and corresponding prefix([SheetNamePrefix](../sheetnameprefix/)) will not be added to the file path. |
| [buildPathWithSplitPartAlways](#buildPathWithSplitPartAlways--)| boolean | Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix([SplitPartPrefix](../splitpartprefix/)) will not be added to the file path. |
| [sheetNamePrefix](#sheetNamePrefix--)| string | Prefix for the index of worksheet. |
| [sheetIndexPrefix](#sheetIndexPrefix--)| string | Prefix for the index of worksheet. |
| [splitPartPrefix](#splitPartPrefix--)| string | Prefix for the index of split part. |
| [saveOptionsTemplate](#saveOptionsTemplate--)| LowCodeSaveOptions | The template for creating instance of save options in [GetSaveOptions(SplitPartInfo)](../getsaveoptions(splitpartinfo)/). |
## Methods
| Method | Description |
| --- | --- |
| [getSheetIndexOffset()](#getSheetIndexOffset--)| <b>@deprecated.</b> Please use the 'sheetIndexOffset' property instead. Offset of sheet's index between what used in file path and its actual value([SplitPartInfo.SheetIndex](../splitpartinfo.sheetindex/)). |
| [setSheetIndexOffset(number)](#setSheetIndexOffset-number-)| <b>@deprecated.</b> Please use the 'sheetIndexOffset' property instead. Offset of sheet's index between what used in file path and its actual value([SplitPartInfo.SheetIndex](../splitpartinfo.sheetindex/)). |
| [getSplitPartIndexOffset()](#getSplitPartIndexOffset--)| <b>@deprecated.</b> Please use the 'splitPartIndexOffset' property instead. Offset of split part's index between what used in file path and its actual value([SplitPartInfo.PartIndex](../splitpartinfo.partindex/)). |
| [setSplitPartIndexOffset(number)](#setSplitPartIndexOffset-number-)| <b>@deprecated.</b> Please use the 'splitPartIndexOffset' property instead. Offset of split part's index between what used in file path and its actual value([SplitPartInfo.PartIndex](../splitpartinfo.partindex/)). |
| [getBuildPathWithSheetAlways()](#getBuildPathWithSheetAlways--)| <b>@deprecated.</b> Please use the 'buildPathWithSheetAlways' property instead. Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index and name and corresponding prefix([SheetNamePrefix](../sheetnameprefix/)) will not be added to the file path. |
| [setBuildPathWithSheetAlways(boolean)](#setBuildPathWithSheetAlways-boolean-)| <b>@deprecated.</b> Please use the 'buildPathWithSheetAlways' property instead. Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index and name and corresponding prefix([SheetNamePrefix](../sheetnameprefix/)) will not be added to the file path. |
| [getBuildPathWithSplitPartAlways()](#getBuildPathWithSplitPartAlways--)| <b>@deprecated.</b> Please use the 'buildPathWithSplitPartAlways' property instead. Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix([SplitPartPrefix](../splitpartprefix/)) will not be added to the file path. |
| [setBuildPathWithSplitPartAlways(boolean)](#setBuildPathWithSplitPartAlways-boolean-)| <b>@deprecated.</b> Please use the 'buildPathWithSplitPartAlways' property instead. Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix([SplitPartPrefix](../splitpartprefix/)) will not be added to the file path. |
| [getSheetNamePrefix()](#getSheetNamePrefix--)| <b>@deprecated.</b> Please use the 'sheetNamePrefix' property instead. Prefix for the index of worksheet. |
| [setSheetNamePrefix(string)](#setSheetNamePrefix-string-)| <b>@deprecated.</b> Please use the 'sheetNamePrefix' property instead. Prefix for the index of worksheet. |
| [getSheetIndexPrefix()](#getSheetIndexPrefix--)| <b>@deprecated.</b> Please use the 'sheetIndexPrefix' property instead. Prefix for the index of worksheet. |
| [setSheetIndexPrefix(string)](#setSheetIndexPrefix-string-)| <b>@deprecated.</b> Please use the 'sheetIndexPrefix' property instead. Prefix for the index of worksheet. |
| [getSplitPartPrefix()](#getSplitPartPrefix--)| <b>@deprecated.</b> Please use the 'splitPartPrefix' property instead. Prefix for the index of split part. |
| [setSplitPartPrefix(string)](#setSplitPartPrefix-string-)| <b>@deprecated.</b> Please use the 'splitPartPrefix' property instead. Prefix for the index of split part. |
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
### constructor(string) {#constructor-string-}
Instantiates an instance to provide save options according to specified templates.
```javascript
constructor(pathTemplate: string);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pathTemplate | string | The template of the resultant file path. |
**Remarks**
The supported placeholders in file path template: <ul> <li>${SheetIndex}: will be replaced by the sheet index of the split part</li> <li>${SheetName}: will be replaced by the sheet name of the split part</li> <li>${SplitPartIndex}: will be replaced by the index of the split part</li> <li>${SheetIndexPrefix}: will be replaced by [SheetIndexPrefix](../sheetindexprefix/)</li> <li>${SheetNamePrefix}: will be replaced by [SheetNamePrefix](../sheetnameprefix/)</li> <li>${SplitPartPrefix}: will be replaced by [SplitPartPrefix](../splitpartprefix/)</li> </ul
### sheetIndexOffset {#sheetIndexOffset--}
Offset of sheet's index between what used in file path and its actual value([SplitPartInfo.SheetIndex](../splitpartinfo.sheetindex/)).
```javascript
sheetIndexOffset : number;
```
### splitPartIndexOffset {#splitPartIndexOffset--}
Offset of split part's index between what used in file path and its actual value([SplitPartInfo.PartIndex](../splitpartinfo.partindex/)).
```javascript
splitPartIndexOffset : number;
```
### buildPathWithSheetAlways {#buildPathWithSheetAlways--}
Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index and name and corresponding prefix([SheetNamePrefix](../sheetnameprefix/)) will not be added to the file path.
```javascript
buildPathWithSheetAlways : boolean;
```
### buildPathWithSplitPartAlways {#buildPathWithSplitPartAlways--}
Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix([SplitPartPrefix](../splitpartprefix/)) will not be added to the file path.
```javascript
buildPathWithSplitPartAlways : boolean;
```
### sheetNamePrefix {#sheetNamePrefix--}
Prefix for the index of worksheet.
```javascript
sheetNamePrefix : string;
```
**Remarks**
If there is only one worksheet and [BuildPathWithSheetAlways](../buildpathwithsheetalways/) is false, then this prefix and the sheet index(or name) will not be added to the resultant file path.
### sheetIndexPrefix {#sheetIndexPrefix--}
Prefix for the index of worksheet.
```javascript
sheetIndexPrefix : string;
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
### saveOptionsTemplate {#saveOptionsTemplate--}
The template for creating instance of save options in [GetSaveOptions(SplitPartInfo)](../getsaveoptions(splitpartinfo)/).
```javascript
saveOptionsTemplate : LowCodeSaveOptions;
```
**Remarks**
If the template has been specified, then the created instance will copy all setting from it and update the output file accordingly.
### getSheetIndexOffset() {#getSheetIndexOffset--}
```javascript
getSheetIndexOffset() : number;
```
### setSheetIndexOffset(number) {#setSheetIndexOffset-number-}
```javascript
setSheetIndexOffset(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
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
### getSheetNamePrefix() {#getSheetNamePrefix--}
```javascript
getSheetNamePrefix() : string;
```
**Remarks**
If there is only one worksheet and [BuildPathWithSheetAlways](../buildpathwithsheetalways/) is false, then this prefix and the sheet index(or name) will not be added to the resultant file path.
### setSheetNamePrefix(string) {#setSheetNamePrefix-string-}
```javascript
setSheetNamePrefix(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
If there is only one worksheet and [BuildPathWithSheetAlways](../buildpathwithsheetalways/) is false, then this prefix and the sheet index(or name) will not be added to the resultant file path.
### getSheetIndexPrefix() {#getSheetIndexPrefix--}
```javascript
getSheetIndexPrefix() : string;
```
**Remarks**
If there is only one worksheet and [BuildPathWithSheetAlways](../buildpathwithsheetalways/) is false, then this prefix and the sheet index(or name) will not be added to the resultant file path.
### setSheetIndexPrefix(string) {#setSheetIndexPrefix-string-}
```javascript
setSheetIndexPrefix(value: string) : void;
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
