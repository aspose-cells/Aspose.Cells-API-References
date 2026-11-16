---
title: "GetHtmlCrossStringType 方法"
linktitle: "GetHtmlCrossStringType"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "GetHtmlCrossStringType 方法。封装了在 Go 中表示 gethtmlcrossstringtype 的函数。"
type: docs
weight: 200
url: /zh/go-cpp/htmlsaveoptions/gethtmlcrossstringtype/
---

## GetHtmlCrossStringType function

指示在将 Excel 文件保存为 html 格式时，跨单元格字符串是否以与 MS Excel 相同的方式显示。默认值为 Default，因此对于跨单元格字符串，Aspose.Cells 创建的 html 文件与 MS Excel 的差别很小。但在创建大型 html 文件时，将值设为 Cross 的性能会比设为 Default 或 Fit2Cell 快数倍。

```go

func (instance *HtmlSaveOptions) GetHtmlCrossStringType()  (HtmlCrossType,  error) 

```

## 备注


## 另请参阅

* Class [HtmlSaveOptions](../)
* Library [Aspose.Cells for Go](../../)
