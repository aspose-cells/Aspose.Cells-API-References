---
title: "RevisionCellMove 类"
linktitle: "RevisionCellMove"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "RevisionCellMove 类。封装在 Go 中表示 revisioncellmove 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/revisioncellmove/
---

## RevisionCellMove class

表示已移动单元格的修订记录。

```go

type RevisionCellMove struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewRevisionCellMove](./newrevisioncellmove/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetType](./gettype/) | 表示修订的类型。 |
| [GetSourceArea](./getsourcearea/) | 获取源区域。 |
| [GetDestinationArea](./getdestinationarea/) | 获取目标区域。 |
| [GetSourceWorksheet](./getsourceworksheet/) | 获取源工作表。 |
| [GetWorksheet](./getworksheet/) | 获取工作表。 |
| [GetId](./getid/) | 获取此修订的编号。 |
