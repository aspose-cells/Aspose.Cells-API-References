---
title: "LowCodePdfSaveOptions 类"
linktitle: "LowCodePdfSaveOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "LowCodePdfSaveOptions 类。封装表示 Go 中 lowcodepdfsaveoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/lowcodepdfsaveoptions/
---

## LowCodePdfSaveOptions class

以低代码方式保存 pdf 的选项。

```go

type LowCodePdfSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewLowCodePdfSaveOptions](./newlowcodepdfsaveoptions/) | 默认构造函数。 |
| [NewLowCodePdfSaveOptions_LowCodeSaveOptions](./newlowcodepdfsaveoptions_lowcodesaveoptions/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetSaveFormat](./getsaveformat/) | 输出的保存格式。转换为 pdf 时，只能是 SaveFormat.Pdf。 |
| [SetSaveFormat](./setsaveformat/) | 输出的保存格式。转换为 pdf 时，只能是 SaveFormat.Pdf。 |
| [GetPdfOptions](./getpdfoptions/) | 保存 Pdf 文件的选项。 |
| [SetPdfOptions](./setpdfoptions/) | 保存 Pdf 文件的选项。 |
| [GetOutputFile](./getoutputfile/) | 获取和设置用于保存生成数据的文件（如有需要包括路径）。当将此属性设置为非 null 或非空字符串时，OutputStream 将被忽略。 |
| [SetOutputFile](./setoutputfile/) | 获取和设置用于保存生成数据的文件（如有需要包括路径）。当将此属性设置为非 null 或非空字符串时，OutputStream 将被忽略。 |
| [GetOutputStream](./getoutputstream/) | 获取和设置用于写入生成数据的流。当将此属性设置为非 null 时，OutputFile 将被忽略。 |
| [SetOutputStream](./setoutputstream/) | 获取和设置用于写入生成数据的流。当将此属性设置为非 null 时，OutputFile 将被忽略。 |
