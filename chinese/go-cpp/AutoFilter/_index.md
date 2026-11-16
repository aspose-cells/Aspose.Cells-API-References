---
title: "AutoFilter 类"
linktitle: "AutoFilter"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "AutoFilter 类。封装在 Go 中表示自动筛选的对象。"
type: docs
weight: 200
url: /zh/go-cpp/autofilter/
---

## AutoFilter class

表示对指定工作表的自动筛选。

```go

type AutoFilter struct  {
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
| [GetSorter](./getsorter/) | 获取数据排序器。 |
| [SetRange_Int_Int_Int](./setrange_int_int_int/) | 设置指定 AutoFilter 所适用的范围。 |
| [GetCellArea](./getcellarea/) | 获取此 AutoFilter 所适用的 CellArea。 |
| [GetCellArea_Bool](./getcellarea_bool/) | 获取指定 AutoFilter 所适用的 Aspose.Cells.CellArea。 |
| [GetRange](./getrange/) | 表示指定 AutoFilter 所适用的范围。 |
| [SetRange_String](./setrange_string/) | 表示指定 AutoFilter 所适用的范围。 |
| [AddFilter](./addfilter/) | 为筛选列添加过滤器。 |
| [AddDateFilter](./adddatefilter/) | 添加日期过滤器。 |
| [RemoveDateFilter](./removedatefilter/) | 移除日期过滤器。 |
| [RemoveFilter_Int_String](./removefilter_int_string/) | 移除筛选列的过滤器。 |
| [Filter](./filter/) | 使用指定条件过滤列表。 |
| [FilterTop10](./filtertop10/) | 过滤列表中前 10 项 |
| [Dynamic_Filter](./dynamic_filter/) | 添加动态过滤器。 |
| [AddFontColorFilter](./addfontcolorfilter/) | 添加字体颜色过滤器。 |
| [AddFillColorFilter](./addfillcolorfilter/) | 添加填充颜色过滤器。 |
| [AddIconFilter](./addiconfilter/) | 添加图标过滤器。 |
| [MatchBlanks](./matchblanks/) | 匹配列表中所有空白单元格。 |
| [MatchNonBlanks](./matchnonblanks/) | 匹配列表中所有非空白单元格。 |
| [Custom_Int_FilterOperatorType_Object](./custom_int_filteroperatortype_object/) | 使用自定义条件过滤列表。 |
| [Custom_Int_FilterOperatorType_Object_Bool_FilterOperatorType_Object](./custom_int_filteroperatortype_object_bool_filteroperatortype_object/) | 使用自定义条件过滤列表。 |
| [ShowAll](./showall/) | 取消隐藏所有行。 |
| [RemoveFilter_Int](./removefilter_int/) | 移除特定过滤器。 |
| [Refresh](./refresh/) | 刷新自动过滤器以隐藏或取消隐藏行。 |
| [Refresh_Bool](./refresh_bool/) | 获取所有隐藏行的索引。 |
| [GetShowFilterButton](./getshowfilterbutton/) | 指示此列的自动筛选按钮是否可见。 |
| [SetShowFilterButton](./setshowfilterbutton/) | 指示此列的自动筛选按钮是否可见。 |
| [GetFilterColumns](./getfiltercolumns/) | 获取过滤列的集合。 |
