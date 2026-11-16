---
title: "DeleteOptions 类"
linktitle: "DeleteOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "DeleteOptions 类。封装在 Go 中表示 deleteoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/deleteoptions/
---

## DeleteOptions class

表示删除行/列的设置。

```go

type DeleteOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewDeleteOptions](./newdeleteoptions/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetUpdateReference](./getupdatereference/) | 指示是否在其他工作表中更新引用。 |
| [SetUpdateReference](./setupdatereference/) | 指示是否在其他工作表中更新引用。 |
| [GetFormulaChangeMonitor](./getformulachangemonitor/) | 获取/设置用于跟踪删除导致的更改的监视器。 |
| [SetFormulaChangeMonitor](./setformulachangemonitor/) | 获取/设置用于跟踪删除导致的更改的监视器。 |
