---
title: "PivotAreaFilter 类"
linktitle: "PivotAreaFilter"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PivotAreaFilter 类。封装在 Go 中表示 pivotareafilter 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/pivotareafilter/
---

## PivotAreaFilter class

表示用于 <see cref="PivotTable"/> 的 <see cref="PivotArea"/> 过滤器。

```go

type PivotAreaFilter struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewPivotAreaFilter](./newpivotareafilter/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [IsSubtotalSet](./issubtotalset/) | 获取此筛选器设置的子总计。 |
| [SetSubtotals](./setsubtotals/) | 筛选器的子总计。 |
| [GetFieldIndex](./getfieldindex/) | 获取此筛选器引用的源字段中字段的索引。-2 的值表示值字段。 |
| [GetSelected](./getselected/) | 指示此字段是否具有选择。仅在数据透视表处于大纲视图时有效。 |
| [SetSelected](./setselected/) | 指示此字段是否具有选择。仅在数据透视表处于大纲视图时有效。 |
