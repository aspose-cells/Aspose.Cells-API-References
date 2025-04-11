---
title: SplitPartInfo
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the information of one inputoutput for multiple inputsoutputs such as current page to be rendered when converting spreadsheet to image.
type: docs
url: /nodejs-cpp/splitpartinfo/
---

## SplitPartInfo class

Represents the information of one input/output for multiple inputs/outputs, such as current page to be rendered when converting spreadsheet to image.

```javascript
class SplitPartInfo;
```


## Methods

| Method | Description |
| --- | --- |
| [getPartIndex()](#getPartIndex--)| Index of current part in sequence(0 based). -1 means there are no multiple parts so the result is single. |
| [getSheetIndex()](#getSheetIndex--)| Index of the sheet where current part is in. -1 denotes there is only one sheet. |
| [getSheetName()](#getSheetName--)| Name of the sheet where current part is in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getPartIndex() {#getPartIndex--}

Index of current part in sequence(0 based). -1 means there are no multiple parts so the result is single.

```javascript
getPartIndex() : number;
```


**Remarks**

If multiple sheets need to be processed and every sheet is processed(split) separately, the part index always starts from 0 for every sheet. For example, when converting workbook to images, it represents the output page index of currently processed sheet. And -1 denotes there is only one page for current sheet.

### getSheetIndex() {#getSheetIndex--}

Index of the sheet where current part is in. -1 denotes there is only one sheet.

```javascript
getSheetIndex() : number;
```


### getSheetName() {#getSheetName--}

Name of the sheet where current part is in.

```javascript
getSheetName() : string;
```


**Remarks**

May be null for some situations, such as when rendering the whole workbook to tiff image.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



