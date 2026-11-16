---
title: "TimelineCollection 类"
linktitle: "TimelineCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "TimelineCollection 类。封装在 Go 中表示 timelinecollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/timelinecollection/
---

## TimelineCollection class

指定工作表上所有 <see cref="Timeline"/> 对象的集合。自 Excel 2013 起支持。

```go

type TimelineCollection struct  {
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
| [Get_Int](./get_int/) | 通过索引获取时间线。 |
| [Get_String](./get_string/) | 通过时间线名称获取时间线。 |
| [Add_PivotTable_Int_Int_String](./add_pivottable_int_int_string/) | 使用 PivotTable 作为数据源添加新的时间线 |
| [Add_PivotTable_String_String](./add_pivottable_string_string/) | 使用 PivotTable 作为数据源添加新的时间线 |
| [Add_PivotTable_Int_Int_Int](./add_pivottable_int_int_int/) | 使用 PivotTable 作为数据源添加新的时间线 |
| [Add_PivotTable_String_Int](./add_pivottable_string_int/) | 使用 PivotTable 作为数据源添加新的时间线 |
| [Add_PivotTable_Int_Int_PivotField](./add_pivottable_int_int_pivotfield/) | 使用 PivotTable 作为数据源添加新的时间线 |
| [Add_PivotTable_String_PivotField](./add_pivottable_string_pivotfield/) | 使用 PivotTable 作为数据源添加新的时间线 |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
