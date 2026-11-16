---
title: "MergedCellsShrinkType 枚举"
linktitle: "MergedCellsShrinkType"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "MergedCellsShrinkType 枚举。封装在 Go 中表示 mergedcellsshrinktype 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/mergedcellsshrinktype/
---

## MergedCellsShrinkType Enum

表示用于删除空行/列等操作时收缩合并单元格的策略。

```go

type MergedCellsShrinkType int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [None](./none/) | 保持合并单元格不变，不进行任何修改。 |
| [ShrinkToFit](./shrinktofit/) | 在需要时收缩合并区域，通过删除底部的行或右侧的列，同时确保所有内容保持可见。 |
| [KeepHeaderOnly](./keepheaderonly/) | 仅在合并区域左上单元格不为空时保留合并区域的标题行/列。 |
