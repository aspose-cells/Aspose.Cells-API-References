---
title: "PivotFieldCollection 类"
linktitle: "PivotFieldCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PivotFieldCollection 类。封装在 Go 中表示 pivotfieldcollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/pivotfieldcollection/
---

## PivotFieldCollection class

表示透视表不同区域中所有 PivotField 对象的集合。

```go

type PivotFieldCollection struct  {
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
| [GetType](./gettype/) | 获取 PivotFields 类型。 |
| [Get_Int](./get_int/) | 获取特定索引处的 PivotField 对象。 |
| [Get_String](./get_string/) | 获取特定名称的 PivotField 对象。 |
| [RemoveAt](./removeat/) | 通过索引移除字段。仅适用于过滤器、行、列、数据区域。 |
| [AddByBaseIndex](./addbybaseindex/) | 向特定类型的 PivotFields 添加 PivotField 对象。 |
| [Add](./add/) | 向特定类型的 PivotFields 添加 PivotField 对象。 |
| [Insert](./insert/) | 在特定索引处插入 pivot field。 |
| [Clear](./clear/) | 清除 PivotFieldCollection 的所有字段 |
| [Remove](./remove/) | 从当前区域移除字段。 |
| [Move](./move/) | 将 PivotField 从当前位置移动到目标位置 |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
