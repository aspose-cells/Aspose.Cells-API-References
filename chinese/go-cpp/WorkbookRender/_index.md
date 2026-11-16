---
title: "WorkbookRender 类"
linktitle: "WorkbookRender"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "WorkbookRender 类。封装了在 Go 中表示 workbookrender 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/workbookrender/
---

## WorkbookRender class

表示工作簿渲染。此类的构造函数必须在修改页面设置、单元格样式后使用。

```go

type WorkbookRender struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewWorkbookRender](./newworkbookrender/) | WorkbookRender 的构造 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetPageCount](./getpagecount/) | 获取工作簿的总页数。 |
| [GetPageSizeInch](./getpagesizeinch/) | 获取输出图像的英寸尺寸。 |
| [ToImage](./toimage/) | 将整个工作簿渲染为 Tiff 图像并输出到流。 |
| [ToImage_String](./toimage_string/) | 将整个工作簿渲染为 Tiff 图像并保存到文件。 |
| [ToImage_Int_String](./toimage_int_string/) | 将指定页面渲染并保存到文件。 |
| [ToImage_Int](./toimage_int/) | 将指定页面渲染并输出到流。 |
| [Dispose](./dispose/) | 释放为渲染创建和使用的资源。 |
