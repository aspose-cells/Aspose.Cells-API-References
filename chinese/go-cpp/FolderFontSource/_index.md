---
title: "FolderFontSource 类"
linktitle: "FolderFontSource"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "FolderFontSource 类。封装在 Go 中表示 folderfontsource 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/folderfontsource/
---

## FolderFontSource class

表示包含 TrueType 字体文件的文件夹。

```go

type FolderFontSource struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewFolderFontSource_String_Bool](./newfolderfontsource_string_bool/) | 构造函数。 |
| [NewFolderFontSource_FontSourceBase](./newfolderfontsource_fontsourcebase/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetFolderPath](./getfolderpath/) | 字体文件夹的路径。 |
| [GetScanSubFolders](./getscansubfolders/) | 确定是否扫描子文件夹。 |
| [GetType](./gettype/) | 返回字体源的类型。 |
