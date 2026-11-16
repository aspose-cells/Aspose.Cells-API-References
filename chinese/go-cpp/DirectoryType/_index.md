---
title: "DirectoryType 枚举"
linktitle: "DirectoryType"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "DirectoryType 枚举。封装在 Go 中表示 directorytype 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/directorytype/
---

## DirectoryType Enum

表示文件名的目录类型。

```go

type DirectoryType int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [Volume](./volume/) | 表示 MS-DOS 驱动器字母。后跟驱动器字母。或 UNC 文件名，例如 \\server\share\myfile.xls |
| [SameVolume](./samevolume/) | 指示源工作簿与依赖工作簿位于同一驱动器上（省略驱动器字母）。 |
| [DownDirectory](./downdirectory/) | 指示源工作簿位于当前目录的子目录中。 |
| [UpDirectory](./updirectory/) | 指示源工作簿位于当前目录的父目录中。 |
