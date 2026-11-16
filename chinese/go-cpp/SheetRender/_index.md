---
title: "SheetRender 类"
linktitle: "SheetRender"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "SheetRender 类。封装在 Go 中表示 sheetRender 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/sheetrender/
---

## SheetRender class

表示工作表渲染，可将工作表渲染为多种图像（如 BMP、PNG、JPEG、TIFF 等）。此类的构造函数必须在修改页面设置、单元格样式后使用。

```go

type SheetRender struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewSheetRender](./newsheetrender/) | 构造 SheetRender，需要 worksheet 和 ImageOrPrintOptions 作为参数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetPageCount](./getpagecount/) | 获取当前工作表的总页数。 |
| [GetPageScale](./getpagescale/) | 获取工作表的计算页缩放比例。如果设置了 PageSetup.Zoom，则返回设定的缩放比例；否则，根据 PageSetup.FitToPagesWide 和 PageSetup.FitToPagesTall 返回计算得到的缩放比例。 |
| [GetPageSizeInch](./getpagesizeinch/) | 获取输出图像的英寸尺寸。 |
| [ToImage_Int_String](./toimage_int_string/) | 将指定页面渲染并保存到文件。 |
| [ToImage_Int](./toimage_int/) | 将指定页面渲染并输出到流。 |
| [ToTiff](./totiff/) | 将整个工作表渲染为 Tiff 图像并输出到流。 |
| [ToTiff_String](./totiff_string/) | 将整个工作表渲染为 Tiff 图像并保存到文件。 |
| [Dispose](./dispose/) | 释放为渲染创建和使用的资源。 |
