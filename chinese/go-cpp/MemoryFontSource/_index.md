---
title: "MemoryFontSource 类"
linktitle: "MemoryFontSource"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "MemoryFontSource 类。封装在 Go 中表示 memoryfontsource 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/memoryfontsource/
---

## MemoryFontSource class

表示存储在内存中的单个 TrueType 字体文件。

```go

type MemoryFontSource struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewMemoryFontSource_Stream](./newmemoryfontsource_stream/) | 构造函数。 |
| [NewMemoryFontSource_FontSourceBase](./newmemoryfontsource_fontsourcebase/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetFontData](./getfontdata/) | 二进制字体数据。 |
| [GetType](./gettype/) | 返回字体源的类型。 |
