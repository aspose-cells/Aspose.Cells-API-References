---
title: LowCodeSaveOptionsProviderOfAssembling
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Implementation to provide save options which save split parts to files and the path of resultant file are named asit may contains directories PathHeader..pathheaderSheetPrefix..sheetprefixSheetIndexor SheetName SplitPartPrefix..splitpartprefixSplitPartIndexPathTail..pathtail.
type: docs
url: /nodejs-cpp/lowcodesaveoptionsproviderofassembling/
---

## LowCodeSaveOptionsProviderOfAssembling class

Implementation to provide save options which save split parts to files and the path of resultant file are named as(it may contains directories): [PathHeader](../pathheader/)+[SheetPrefix](../sheetprefix/)+SheetIndex(or SheetName) +[SplitPartPrefix](../splitpartprefix/)+SplitPartIndex+[PathTail](../pathtail/).

```javascript
class LowCodeSaveOptionsProviderOfAssembling extends AbstractLowCodeSaveOptionsProvider;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(AbstractLowCodeSaveOptionsProvider)](#constructor-abstractlowcodesaveoptionsprovider-)| Constructs from a parent object convertible to this. |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getPathHeader()](#getPathHeader--)| Header part(before added content of sheet and split part) of file path. |
| [setPathHeader(string)](#setPathHeader-string-)| Header part(before added content of sheet and split part) of file path. |
| [getPathTail()](#getPathTail--)| Tailing part(after sequence numbers) of file path. It should include extension of file name. |
| [setPathTail(string)](#setPathTail-string-)| Tailing part(after sequence numbers) of file path. It should include extension of file name. |
| [getUseSheetName()](#getUseSheetName--)| Whether builds the file path with sheet name instead of sheet index. Default value is false. |
| [setUseSheetName(boolean)](#setUseSheetName-boolean-)| Whether builds the file path with sheet name instead of sheet index. Default value is false. |
| [getSheetPrefix()](#getSheetPrefix--)| Prefix for the index of worksheet. |
| [setSheetPrefix(string)](#setSheetPrefix-string-)| Prefix for the index of worksheet. |
| [getSplitPartPrefix()](#getSplitPartPrefix--)| Prefix for the index of split part. |
| [setSplitPartPrefix(string)](#setSplitPartPrefix-string-)| Prefix for the index of split part. |
| [getSheetIndexOffset()](#getSheetIndexOffset--)| Offset of sheet's index between what used in file path and its actual value([SplitPartInfo.SheetIndex](../splitpartinfo.sheetindex/)). |
| [setSheetIndexOffset(number)](#setSheetIndexOffset-number-)| Offset of sheet's index between what used in file path and its actual value([SplitPartInfo.SheetIndex](../splitpartinfo.sheetindex/)). |
| [getSplitPartIndexOffset()](#getSplitPartIndexOffset--)| Offset of split part's index between what used in file path and its actual value([SplitPartInfo.PartIndex](../splitpartinfo.partindex/)). |
| [setSplitPartIndexOffset(number)](#setSplitPartIndexOffset-number-)| Offset of split part's index between what used in file path and its actual value([SplitPartInfo.PartIndex](../splitpartinfo.partindex/)). |
| [getBuildPathWithSheetAlways()](#getBuildPathWithSheetAlways--)| Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index(or name) and corresponding prefix will not be added to the file path. |
| [setBuildPathWithSheetAlways(boolean)](#setBuildPathWithSheetAlways-boolean-)| Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index(or name) and corresponding prefix will not be added to the file path. |
| [getBuildPathWithSplitPartAlways()](#getBuildPathWithSplitPartAlways--)| Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix will not be added to the file path. |
| [setBuildPathWithSplitPartAlways(boolean)](#setBuildPathWithSplitPartAlways-boolean-)| Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix will not be added to the file path. |
| [getSaveOptionsTemplate()](#getSaveOptionsTemplate--)| The template for creating instance of save options in [GetSaveOptions(SplitPartInfo)](../getsaveoptions(splitpartinfo)/). |
| [setSaveOptionsTemplate(LowCodeSaveOptions)](#setSaveOptionsTemplate-lowcodesaveoptions-)| The template for creating instance of save options in [GetSaveOptions(SplitPartInfo)](../getsaveoptions(splitpartinfo)/). |
| [getSaveOptions(SplitPartInfo)](#getSaveOptions-splitpartinfo-)| Gets the save options from which to get the output settings for currently split part. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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


### getPathHeader() {#getPathHeader--}

Header part(before added content of sheet and split part) of file path.

```javascript
getPathHeader() : string;
```


### setPathHeader(string) {#setPathHeader-string-}

Header part(before added content of sheet and split part) of file path.

```javascript
setPathHeader(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getPathTail() {#getPathTail--}

Tailing part(after sequence numbers) of file path. It should include extension of file name.

```javascript
getPathTail() : string;
```


### setPathTail(string) {#setPathTail-string-}

Tailing part(after sequence numbers) of file path. It should include extension of file name.

```javascript
setPathTail(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getUseSheetName() {#getUseSheetName--}

Whether builds the file path with sheet name instead of sheet index. Default value is false.

```javascript
getUseSheetName() : boolean;
```


**Remarks**

The sheet name will never be rebuilt automatically. So when set it to true, please make sure there is no special sheet name that can cause invalid file path or name.

### setUseSheetName(boolean) {#setUseSheetName-boolean-}

Whether builds the file path with sheet name instead of sheet index. Default value is false.

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

Prefix for the index of worksheet.

```javascript
getSheetPrefix() : string;
```


**Remarks**

If there is only one worksheet and [BuildPathWithSheetAlways](../buildpathwithsheetalways/) is false, then this prefix and the sheet index(or name) will not be added to the resultant file path.

### setSheetPrefix(string) {#setSheetPrefix-string-}

Prefix for the index of worksheet.

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

Prefix for the index of split part.

```javascript
getSplitPartPrefix() : string;
```


**Remarks**

If there is only one split part and [BuildPathWithSplitPartAlways](../buildpathwithsplitpartalways/) is false, then this prefix and the split part index(0) will not be added to the resultant file path.

### setSplitPartPrefix(string) {#setSplitPartPrefix-string-}

Prefix for the index of split part.

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

Offset of sheet's index between what used in file path and its actual value([SplitPartInfo.SheetIndex](../splitpartinfo.sheetindex/)).

```javascript
getSheetIndexOffset() : number;
```


**Remarks**

Only takes effect when [UseSheetName](../usesheetname/) is false.

### setSheetIndexOffset(number) {#setSheetIndexOffset-number-}

Offset of sheet's index between what used in file path and its actual value([SplitPartInfo.SheetIndex](../splitpartinfo.sheetindex/)).

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

Offset of split part's index between what used in file path and its actual value([SplitPartInfo.PartIndex](../splitpartinfo.partindex/)).

```javascript
getSplitPartIndexOffset() : number;
```


### setSplitPartIndexOffset(number) {#setSplitPartIndexOffset-number-}

Offset of split part's index between what used in file path and its actual value([SplitPartInfo.PartIndex](../splitpartinfo.partindex/)).

```javascript
setSplitPartIndexOffset(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getBuildPathWithSheetAlways() {#getBuildPathWithSheetAlways--}

Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index(or name) and corresponding prefix will not be added to the file path.

```javascript
getBuildPathWithSheetAlways() : boolean;
```


### setBuildPathWithSheetAlways(boolean) {#setBuildPathWithSheetAlways-boolean-}

Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index(or name) and corresponding prefix will not be added to the file path.

```javascript
setBuildPathWithSheetAlways(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getBuildPathWithSplitPartAlways() {#getBuildPathWithSplitPartAlways--}

Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix will not be added to the file path.

```javascript
getBuildPathWithSplitPartAlways() : boolean;
```


### setBuildPathWithSplitPartAlways(boolean) {#setBuildPathWithSplitPartAlways-boolean-}

Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix will not be added to the file path.

```javascript
setBuildPathWithSplitPartAlways(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSaveOptionsTemplate() {#getSaveOptionsTemplate--}

The template for creating instance of save options in [GetSaveOptions(SplitPartInfo)](../getsaveoptions(splitpartinfo)/).

```javascript
getSaveOptionsTemplate() : LowCodeSaveOptions;
```


**Returns**

[LowCodeSaveOptions](../lowcodesaveoptions/)

**Remarks**

If the template has been specified, then the created instance will copy all setting from it and update the output file accordingly.

### setSaveOptionsTemplate(LowCodeSaveOptions) {#setSaveOptionsTemplate-lowcodesaveoptions-}

The template for creating instance of save options in [GetSaveOptions(SplitPartInfo)](../getsaveoptions(splitpartinfo)/).

```javascript
setSaveOptionsTemplate(value: LowCodeSaveOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LowCodeSaveOptions](../lowcodesaveoptions/) | The value to set. |

**Remarks**

If the template has been specified, then the created instance will copy all setting from it and update the output file accordingly.

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

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


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


