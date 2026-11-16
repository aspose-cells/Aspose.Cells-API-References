---
title: "DataSorter 类"
linktitle: "DataSorter"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "DataSorter 类。封装了在 Go 中表示 datasorter 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/datasorter/
---

## DataSorter class

DataSorter 的摘要描述。

```go

type DataSorter struct  {
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
| [GetKeys](./getkeys/) | 获取 data sorter 的键列表。 |
| [Clear](./clear/) | 清除所有设置。 |
| [GetHasHeaders](./gethasheaders/) | 表示该范围是否具有标题。 |
| [SetHasHeaders](./sethasheaders/) | 表示该范围是否具有标题。 |
| [AddKey_Int_SortOrder](./addkey_int_sortorder/) | 添加已排序的列索引和排序顺序。 |
| [AddKey_Int_SortOrder_String](./addkey_int_sortorder_string/) | 添加已排序的列索引和排序顺序（自定义排序列表）。 |
| [AddColorKey](./addcolorkey/) | 添加颜色排序键。 |
| [AddKey_Int_SortOnType_SortOrder_Object](./addkey_int_sortontype_sortorder_object/) | 添加已排序的列索引和排序顺序（自定义排序列表）。 |
| [AddKey_Int_SortOrder_stringArray](./addkey_int_sortorder_stringarray/) | 添加已排序的列索引和排序顺序（自定义排序列表）。 |
| [GetKey1](./getkey1/) | 表示第一个已排序列的索引（绝对位置，列 A 为 0，B 为 1，...）。 |
| [SetKey1](./setkey1/) | 表示第一个已排序列的索引（绝对位置，列 A 为 0，B 为 1，...）。 |
| [GetOrder1](./getorder1/) | 表示第一个键的排序顺序。 |
| [SetOrder1](./setorder1/) | 表示第一个键的排序顺序。 |
| [GetKey2](./getkey2/) | 表示第二个已排序列的索引（绝对位置，列 A 为 0，B 为 1，...）。 |
| [SetKey2](./setkey2/) | 表示第二个已排序列的索引（绝对位置，列 A 为 0，B 为 1，...）。 |
| [GetOrder2](./getorder2/) | 表示第二个键的排序顺序。 |
| [SetOrder2](./setorder2/) | 表示第二个键的排序顺序。 |
| [GetKey3](./getkey3/) | 表示第三个已排序列的索引（绝对位置，列 A 为 0，B 为 1，...）。 |
| [SetKey3](./setkey3/) | 表示第三个已排序列的索引（绝对位置，列 A 为 0，B 为 1，...）。 |
| [GetOrder3](./getorder3/) | 表示第三个键的排序顺序。 |
| [SetOrder3](./setorder3/) | 表示第三个键的排序顺序。 |
| [GetSortLeftToRight](./getsortlefttoright/) | True 表示排序方向从左到右。False 表示排序方向从上到下。默认值为 false。 |
| [SetSortLeftToRight](./setsortlefttoright/) | True 表示排序方向从左到右。False 表示排序方向从上到下。默认值为 false。 |
| [GetCaseSensitive](./getcasesensitive/) | 获取和设置比较字符串时是否区分大小写。 |
| [SetCaseSensitive](./setcasesensitive/) | 获取和设置比较字符串时是否区分大小写。 |
| [GetSortAsNumber](./getsortasnumber/) | 指示是否对看起来像数字的内容进行排序。 |
| [SetSortAsNumber](./setsortasnumber/) | 指示是否对看起来像数字的内容进行排序。 |
| [Sort_Cells_Int_Int_Int_Int](./sort_cells_int_int_int_int/) | 对区域的数据进行排序。 |
| [Sort_Cells_CellArea](./sort_cells_cellarea/) | 对区域的数据进行排序。 |
| [Sort](./sort/) | 对范围内的数据进行排序。 |
