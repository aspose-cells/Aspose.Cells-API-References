---
title: "FileFontSource 类"
linktitle: "FileFontSource"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "FileFontSource 类。封装在 Go 中表示 filefontsource 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/filefontsource/
---

## FileFontSource class

表示存储在文件系统中的单个 TrueType 字体文件。

```go

type FileFontSource struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewFileFontSource_String](./newfilefontsource_string/) | 构造函数。 |
| [NewFileFontSource_FontSourceBase](./newfilefontsource_fontsourcebase/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetFilePath](./getfilepath/) | 字体文件的路径。 |
| [GetType](./gettype/) | 返回字体源的类型。 |
