---
title: "ReConnectionMethodType 枚举"
linktitle: "ReConnectionMethodType"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ReConnectionMethodType 枚举。封装了在 Go 中表示 reconnectionMethodType 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/reconnectionmethodtype/
---

## ReConnectionMethodType Enum

指定电子表格应用程序在连接失败时应执行的操作。

```go

type ReConnectionMethodType int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [Required](./required/) | 刷新时使用现有的连接信息，如果它变为无效，则从外部连接文件获取更新的连接信息（如果可用）。 |
| [Always](./always/) | 每次刷新时，从外部连接文件获取更新的连接信息（如果可用），并使用它替代现有的连接信息。如果外部连接文件不可用，则数据刷新将失败。 |
| [Never](./never/) | 即使外部连接文件可用，且现有连接信息无效，也永不从外部连接文件获取更新的连接信息。 |
