---
title: "LowCodeSaveOptions 类"
linktitle: "LowCodeSaveOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "LowCodeSaveOptions 类。封装在 Go 中表示 lowcodesaveoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/lowcodesaveoptions/
---

## LowCodeSaveOptions class

以低代码方式保存生成结果的选项。

```go

type LowCodeSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewLowCodeSaveOptions](./newlowcodesaveoptions/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetOutputFile](./getoutputfile/) | 获取和设置用于保存生成数据的文件（如有需要包括路径）。当将此属性设置为非 null 或非空字符串时，OutputStream 将被忽略。 |
| [SetOutputFile](./setoutputfile/) | 获取和设置用于保存生成数据的文件（如有需要包括路径）。当将此属性设置为非 null 或非空字符串时，OutputStream 将被忽略。 |
| [GetOutputStream](./getoutputstream/) | 获取和设置用于写入生成数据的流。当将此属性设置为非 null 时，OutputFile 将被忽略。 |
| [SetOutputStream](./setoutputstream/) | 获取和设置用于写入生成数据的流。当将此属性设置为非 null 时，OutputFile 将被忽略。 |
| [GetSaveFormat](./getsaveformat/) | 获取并设置输出的保存格式。通常，对于低代码方式的特定处理，只允许使用某些特定格式。请为相应的处理指定正确的格式，否则可能导致意外结果甚至异常。 |
| [SetSaveFormat](./setsaveformat/) | 获取并设置输出的保存格式。通常，对于低代码方式的特定处理，只允许使用某些特定格式。请为相应的处理指定正确的格式，否则可能导致意外结果甚至异常。 |
