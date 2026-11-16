---
title: "PivotFieldSortSetting 类"
linktitle: "PivotFieldSortSetting"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PivotFieldSortSetting 类。封装表示 Go 中 pivotfieldsortsetting 对象。"
type: docs
weight: 200
url: /zh/go-cpp/pivotfieldsortsetting/
---

## PivotFieldSortSetting class

表示透视字段的排序设置。

```go

type PivotFieldSortSetting struct  {
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
| [GetSortType](./getsorttype/) | 表示 SortOrder。 |
| [SetSortType](./setsorttype/) | 表示 SortOrder。 |
| [IsSortByLabels](./issortbylabels/) | 指示是否按字段自身或数据字段进行排序。 |
| [GetSortBy](./getsortby/) | 表示排序字段的索引。-1 表示按透视项自身的值排序。大于或等于零时，表示数据区域中数据字段的索引。 |
| [SetSortBy](./setsortby/) | 表示排序字段的索引。-1 表示按透视项自身的值排序。大于或等于零时，表示数据区域中数据字段的索引。 |
| [GetLineTypeSortedBy](./getlinetypesortedby/) | 用于排序的透视行类型。 |
| [IsSimpleSort](./issimplesort/) | 指示是否将应用简单的数据排序操作。 |
| [SetIsSimpleSort](./setissimplesort/) | 指示是否将应用简单的数据排序操作。 |
| [GetCell](./getcell/) | 按行或列的值进行排序。 |
