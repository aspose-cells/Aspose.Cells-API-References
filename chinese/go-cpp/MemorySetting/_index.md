---
title: "MemorySetting 枚举"
linktitle: "MemorySetting"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "MemorySetting 枚举。封装了在 Go 中表示 memorysetting 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/memorysetting/
---

## MemorySetting Enum

单元格数据模型的内存使用模式。

```go

type MemorySetting int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [Normal](./normal/) | 单元格模型的默认模式。 |
| [MemoryPreference](./memorypreference/) | 更倾向于内存性能。 |
| [FileCache](./filecache/) | 更倾向于内存性能，并使用文件而非内存来维护单元格数据。 |
