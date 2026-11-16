---
title: "RevisionCellComment 类"
linktitle: "RevisionCellComment"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "RevisionCellComment 类。封装了在 Go 中表示修订单元格注释的对象。"
type: docs
weight: 200
url: /zh/go-cpp/revisioncellcomment/
---

## RevisionCellComment class

表示单元格批注更改的修订记录。

```go

type RevisionCellComment struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewRevisionCellComment](./newrevisioncellcomment/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetType](./gettype/) | 获取修订的类型。 |
| [GetRow](./getrow/) | 获取包含注释的行索引。 |
| [GetColumn](./getcolumn/) | 获取包含注释的列索引。 |
| [GetCellName](./getcellname/) | 获取单元格的名称。 |
| [SetCellName](./setcellname/) | 获取单元格的名称。 |
| [GetActionType](./getactiontype/) | 获取修订的操作类型。 |
| [IsOldComment](./isoldcomment/) | 指示它是否是旧注释。 |
| [GetOldLength](./getoldlength/) | 获取此修订中添加的注释文本的长度。 |
| [GetNewLength](./getnewlength/) | 获取此修订之前的注释长度。 |
| [GetWorksheet](./getworksheet/) | 获取工作表。 |
| [GetId](./getid/) | 获取此修订的编号。 |
