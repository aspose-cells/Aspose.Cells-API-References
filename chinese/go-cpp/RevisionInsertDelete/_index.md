---
title: "RevisionInsertDelete 类"
linktitle: "RevisionInsertDelete"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "RevisionInsertDelete 类。封装在 Go 中表示 revisioninsertdelete 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/revisioninsertdelete/
---

## RevisionInsertDelete class

表示行/列插入/删除操作的修订记录。

```go

type RevisionInsertDelete struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewRevisionInsertDelete](./newrevisioninsertdelete/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetType](./gettype/) | 表示修订的类型。 |
| [GetCellArea](./getcellarea/) | 获取插入/删除范围。 |
| [GetActionType](./getactiontype/) | 获取此修订的操作类型。 |
| [GetRevisions](./getrevisions/) | 获取此操作的修订列表。 |
| [GetWorksheet](./getworksheet/) | 获取工作表。 |
| [GetId](./getid/) | 获取此修订的编号。 |
