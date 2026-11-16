---
title: "AbstractLowCodeSaveOptionsProvider 类"
linktitle: "AbstractLowCodeSaveOptionsProvider"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "AbstractLowCodeSaveOptionsProvider 类。封装在 Go 中表示 abstractlowcodesaveoptionsprovider 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/abstractlowcodesaveoptionsprovider/
---

## AbstractLowCodeSaveOptionsProvider class

实现提供多保存选项以满足需要多个输出的过程。例如，<see cref=\"SpreadsheetSplitter\"/> 功能需要多个目标来保存拆分文件。

```go

type AbstractLowCodeSaveOptionsProvider struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetSaveOptions](./getsaveoptions/) | 获取用于获取当前拆分部分输出设置的保存选项。返回 null 表示跳过给定的部分。 |
| [Finish](./finish/) | 在处理当前拆分部分后释放资源。 |
