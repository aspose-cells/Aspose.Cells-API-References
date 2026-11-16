---
title: "SetImageResample 方法"
linktitle: "SetImageResample"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "SetImageResample 方法。封装了在 Go 中表示 setimageresample 的函数。"
type: docs
weight: 200
url: /zh/go-cpp/pdfsaveoptions/setimageresample/
---

## SetImageResample function

设置重新采样图像的目标 PPI（每英寸像素）和 JPEG 质量。所有图像将转换为 JPEG，使用指定的质量设置；大于指定 PPI（每英寸像素）的图像将被重新采样。

```go

func (instance *PdfSaveOptions) SetImageResample(desiredppi int32, jpegquality int32)  error

```

## 备注


## 另请参阅

* Class [PdfSaveOptions](../)
* Library [Aspose.Cells for Go](../../)
