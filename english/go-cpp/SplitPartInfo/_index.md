---
title: SplitPartInfo Class 
linktitle: SplitPartInfo
second_title: Aspose.Cells for Go via C++ API Reference
description: 'SplitPartInfo class. Encapsulates the object that represents splitpartinfo in Go.'
type: docs
weight: 200
url: /go-cpp/splitpartinfo/
---

## SplitPartInfo class

Represents the information of one input/output for multiple inputs/outputs,such as current page to be rendered when converting spreadsheet to image.

```go

type SplitPartInfo struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetPartIndex](./getpartindex/) | Index of current part in sequence(0 based).-1 means there are no multiple parts so the result is single. | 
|[GetSheetIndex](./getsheetindex/) | Index of the sheet where current part is in. -1 denotes there is only one sheet. | 
|[GetSheetName](./getsheetname/) | Name of the sheet where current part is in. | 
