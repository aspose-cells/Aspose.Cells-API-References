---
title: "RevisionQueryTable 类"
linktitle: "RevisionQueryTable"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "RevisionQueryTable 类。封装在 Go 中表示 revisionquerytable 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/revisionquerytable/
---

## RevisionQueryTable class

表示查询表字段更改的修订。

```go

type RevisionQueryTable struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewRevisionQueryTable](./newrevisionquerytable/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetType](./gettype/) | 表示修订的类型。 |
| [GetCellArea](./getcellarea/) | 获取受影响查询表的位置。 |
| [GetFieldId](./getfieldid/) | 获取被删除的特定查询表字段的 ID。 |
| [GetWorksheet](./getworksheet/) | 获取工作表。 |
| [GetId](./getid/) | 获取此修订的编号。 |
