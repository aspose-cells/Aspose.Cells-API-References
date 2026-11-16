---
title: "FilterColumn 类"
linktitle: "FilterColumn"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "FilterColumn 类。封装了在 Go 中表示 filtercolumn 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/filtercolumn/
---

## FilterColumn class

表示单列或表中列的筛选器。

```go

type FilterColumn struct  {
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
| [IsDropdownVisible](./isdropdownvisible/) | 指示此列的自动筛选按钮是否可见。 |
| [SetIsDropdownVisible](./setisdropdownvisible/) | 指示此列的自动筛选按钮是否可见。 |
| [GetFilterType](./getfiltertype/) | 获取并设置过滤数据的类型。 |
| [SetFilterType](./setfiltertype/) | 获取并设置过滤数据的类型。 |
| [GetFilterValues](./getfiltervalues/) | 获取 Aspose.Cells.FilterValueCollection，用于按标签或日期时间过滤数据。 |
| [GetCustomFilters](./getcustomfilters/) | 获取 CustomFilterCollection，用于按自定义条件过滤数据。 |
| [SetCustomFilters](./setcustomfilters/) | 获取 CustomFilterCollection，用于按自定义条件过滤数据。 |
| [GetColorFilter](./getcolorfilter/) | 获取 Aspose.Cells.ColorFilter，用于按颜色过滤数据。 |
| [GetDynamicFilter](./getdynamicfilter/) | 获取 DynamicFilter，用于使用动态条件进行过滤。 |
| [GetIconFilter](./geticonfilter/) | 获取 IconFilter，用于按图标过滤数据。 |
| [GetTop10Filter](./gettop10filter/) | 获取 Top10Filter，用于按数据排名进行过滤。 |
| [GetFieldIndex](./getfieldindex/) | 获取并设置范围内的列偏移量。 |
| [SetFieldIndex](./setfieldindex/) | 获取并设置范围内的列偏移量。 |
| [SelectAll](./selectall/) | 全选。 |
