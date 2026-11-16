---
title: "GetDefaultFont 方法"
linktitle: "GetDefaultFont"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "GetDefaultFont 方法。封装了在 Go 中表示 getdefaultfont 的函数。"
type: docs
weight: 200
url: /zh/go-cpp/pptxsaveoptions/getdefaultfont/
---

## GetDefaultFont function

当 Excel 中的字符是 Unicode 且单元格样式未设置正确字体时，它们可能在 pdf、图像中显示为方块。请将 DefaultFont 设置为如 MingLiu 或 MS Gothic 等字体以显示这些字符。如果未设置此属性，Aspose.Cells 将使用系统默认字体来显示这些 Unicode 字符。

```go

func (instance *PptxSaveOptions) GetDefaultFont()  (string,  error) 

```

## 备注


## 另请参阅

* Class [PptxSaveOptions](../)
* Library [Aspose.Cells for Go](../../)
