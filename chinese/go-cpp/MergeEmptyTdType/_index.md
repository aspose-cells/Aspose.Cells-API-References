---
title: "MergeEmptyTdType 枚举"
linktitle: "MergeEmptyTdType"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "MergeEmptyTdType 枚举。封装在 Go 中表示 mergeemptytdtype 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/mergeemptytdtype/
---

## MergeEmptyTdType Enum

表示在导出文件为 HTML 时空 TD 元素的合并类型。

```go

type MergeEmptyTdType int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [Default](./default/) | 显示效果类似于 MS Excel。 |
| [None](./none/) | 导出文件为 HTML 时，空的 TD 元素将不会被合并。这会生成显著更大的 HTML 文件。 |
| [MergeForcely](./mergeforcely/) | 导出文件为 HTML 时强制合并空的 TD 元素。将值设为 true 后，HTML 文件大小会显著减小。如果希望将 HTML 文件导入 Excel，或在保存为 HTML 时导出完美的网格线，请保持默认值。 |
