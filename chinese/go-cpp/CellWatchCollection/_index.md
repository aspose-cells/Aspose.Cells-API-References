---
title: "CellWatchCollection 类"
linktitle: "CellWatchCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "CellWatchCollection 类。封装在 Go 中表示 cellwatchcollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/cellwatchcollection/
---

## CellWatchCollection class

表示在‘监视窗口’中被监视的此工作表上的单元格集合。

```go

type CellWatchCollection struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewCellWatchCollection](./newcellwatchcollection/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [Add_Int_Int](./add_int_int/) | 添加具有行和列的 Aspose.Cells.CellWatch。 |
| [Add_String](./add_string/) | 添加使用单元格名称的 Aspose.Cells.CellWatch。 |
| [Get_Int](./get_int/) | 通过索引获取和设置 CellWatch。 |
| [Get_String](./get_string/) | 通过单元格名称获取和设置 CellWatch。 |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
