﻿---
title: AbstractLowCodeSaveOptionsProvider
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Implementation to provide multiple save options for processes that require multiple outputs. For example SpreadsheetSplitter..spreadsheetsplitter feature requires multiple destinations to save the split files.
type: docs
url: /nodejs-cpp/abstractlowcodesaveoptionsprovider/
---

## AbstractLowCodeSaveOptionsProvider class

Implementation to provide multiple save options for processes that require multiple outputs. For example, [SpreadsheetSplitter](../spreadsheetsplitter/) feature requires multiple destinations to save the split files.

```javascript
class AbstractLowCodeSaveOptionsProvider;
```


## Methods

| Method | Description |
| --- | --- |
| [getSaveOptions(SplitPartInfo)](#getSaveOptions-splitpartinfo-)| Gets the save options from which to get the output settings for currently split part. Returning null denotes to skip given part. |
| [finish(LowCodeSaveOptions)](#finish-lowcodesaveoptions-)| Releases resources after processing currently split part. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getSaveOptions(SplitPartInfo) {#getSaveOptions-splitpartinfo-}

Gets the save options from which to get the output settings for currently split part. Returning null denotes to skip given part.

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

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



