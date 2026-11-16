---
title: "RevisionCellChange 类"
linktitle: "RevisionCellChange"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "RevisionCellChange 类。封装在 Go 中表示 revisioncellchange 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/revisioncellchange/
---

## RevisionCellChange class

表示更改单元格的修订。

```go

type RevisionCellChange struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewRevisionCellChange](./newrevisioncellchange/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetType](./gettype/) | 表示修订的类型。 |
| [GetCellName](./getcellname/) | 获取单元格的名称。 |
| [GetRow](./getrow/) | 获取单元格的行索引。 |
| [GetColumn](./getcolumn/) | 获取单元格的列索引。 |
| [IsNewFormatted](./isnewformatted/) | 指示此单元格是否为新格式化。 |
| [IsOldFormatted](./isoldformatted/) | 指示此单元格是否为旧格式化。 |
| [GetOldFormula](./getoldformula/) | 获取旧公式。 |
| [GetOldValue](./getoldvalue/) | 获取单元格的旧值。 |
| [GetNewValue](./getnewvalue/) | 获取单元格的新值。 |
| [GetNewFormula](./getnewformula/) | 获取旧公式。 |
| [GetNewStyle](./getnewstyle/) | 获取单元格的新样式。 |
| [GetOldStyle](./getoldstyle/) | 获取单元格的旧样式。 |
| [GetWorksheet](./getworksheet/) | 获取工作表。 |
| [GetId](./getid/) | 获取此修订的编号。 |
