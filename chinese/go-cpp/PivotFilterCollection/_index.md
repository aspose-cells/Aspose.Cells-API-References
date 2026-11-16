---
title: "PivotFilterCollection 类"
linktitle: "PivotFilterCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PivotFilterCollection 类。封装了在 Go 中表示 pivotfiltercollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/pivotfiltercollection/
---

## PivotFilterCollection class

表示所有 PivotFilter 的集合。

```go

type PivotFilterCollection struct  {
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
| [Get](./get/) | 获取特定索引处的 pivotfilter 对象。 |
| [AddTop10Filter](./addtop10filter/) | 按数据透视字段的值进行过滤。 |
| [AddValueFilter](./addvaluefilter/) | 按数据透视字段的值进行过滤。 |
| [AddLabelFilter](./addlabelfilter/) | 按行或列透视字段的标题进行过滤。 |
| [AddDateFilter](./adddatefilter/) | 按行或列透视字段的日期设置进行过滤。 |
| [ClearFilter](./clearfilter/) | 从特定的 PivotField 中清除 PivotFilter |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
