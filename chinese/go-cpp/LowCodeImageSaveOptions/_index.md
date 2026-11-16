---
title: "LowCodeImageSaveOptions 类"
linktitle: "LowCodeImageSaveOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "LowCodeImageSaveOptions 类。封装在 Go 中表示 lowcodeimagesaveoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/lowcodeimagesaveoptions/
---

## LowCodeImageSaveOptions class

以低代码方式保存图像的选项。

```go

type LowCodeImageSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewLowCodeImageSaveOptions](./newlowcodeimagesaveoptions/) | 默认构造函数。 |
| [NewLowCodeImageSaveOptions_LowCodeSaveOptions](./newlowcodeimagesaveoptions_lowcodesaveoptions/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetSaveFormat](./getsaveformat/) | 获取或设置保存格式。 |
| [SetSaveFormat](./setsaveformat/) | 获取或设置保存格式。 |
| [GetImageOptions](./getimageoptions/) | 渲染图像的选项。 |
| [SetImageOptions](./setimageoptions/) | 渲染图像的选项。 |
| [GetSaveOptionsProvider](./getsaveoptionsprovider/) | 生成图像的保存选项提供程序。 |
| [SetSaveOptionsProvider](./setsaveoptionsprovider/) | 生成图像的保存选项提供程序。 |
| [GetOutputFile](./getoutputfile/) | 获取和设置用于保存生成数据的文件（如有需要包括路径）。当将此属性设置为非 null 或非空字符串时，OutputStream 将被忽略。 |
| [SetOutputFile](./setoutputfile/) | 获取和设置用于保存生成数据的文件（如有需要包括路径）。当将此属性设置为非 null 或非空字符串时，OutputStream 将被忽略。 |
| [GetOutputStream](./getoutputstream/) | 获取和设置用于写入生成数据的流。当将此属性设置为非 null 时，OutputFile 将被忽略。 |
| [SetOutputStream](./setoutputstream/) | 获取和设置用于写入生成数据的流。当将此属性设置为非 null 时，OutputFile 将被忽略。 |
