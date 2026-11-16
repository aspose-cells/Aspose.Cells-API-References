---
title: "FileFormatInfo 类"
linktitle: "FileFormatInfo"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "FileFormatInfo 类。封装在 Go 中表示 fileformatinfo 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/fileformatinfo/
---

## FileFormatInfo class

包含由 <see cref=\"FileFormatUtil\"/> 文件格式检测方法返回的数据。

```go

type FileFormatInfo struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewFileFormatInfo](./newfileformatinfo/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [IsProtectedByRMS](./isprotectedbyrms/) | 指示文件是否受 Microsoft Rights Management Server 保护。 |
| [IsEncrypted](./isencrypted/) | 如果文档已加密且需要密码打开，则返回 true。 |
| [GetFileFormatType](./getfileformattype/) | 获取检测到的文件格式。 |
| [GetLoadFormat](./getloadformat/) | 获取检测到的加载格式。 |
