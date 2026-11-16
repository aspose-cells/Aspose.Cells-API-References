---
title: "PivotItemCollection 类"
linktitle: "PivotItemCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PivotItemCollection 类。封装在 Go 中表示 pivotitemcollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/pivotitemcollection/
---

## PivotItemCollection class

表示 PivotField 中的所有 <see cref="PivotItem"/> 对象。

```go

type PivotItemCollection struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [Get_Int](./get_int/) | 获取特定索引处的 PivotItem 对象。 |
| [HideAllDetail](./hidealldetail/) | 设置是否隐藏枢轴字段中所有 PivotItems 的所有细节。这是折叠/展开此字段。 |
| [Get_String](./get_string/) | 通过特定名称获取 PivotItem。 |
| [SwapItem](./swapitem/) | 直接交换两个项。 |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
