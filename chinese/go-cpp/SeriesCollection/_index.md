---
title: "SeriesCollection 类"
linktitle: "SeriesCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "SeriesCollection 类。封装在 Go 中表示 seriescollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/seriescollection/
---

## SeriesCollection class

封装 <see cref=\"Series\"/> 对象的集合。

```go

type SeriesCollection struct  {
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
| [Get](./get/) | 获取指定索引处的 Series 元素。 |
| [GetSeriesByOrder](./getseriesbyorder/) | 按顺序获取 Series 元素。 |
| [RemoveAt](./removeat/) | 在特定索引处移除系列。 |
| [GetCategoryData](./getcategorydata/) | 获取或设置类别轴值的范围。它可以是单元格范围（例如 "d1:e10"）或值序列（例如 "{2,6,8,10}"）。 |
| [SetCategoryData](./setcategorydata/) | 获取或设置类别轴值的范围。它可以是单元格范围（例如 "d1:e10"）或值序列（例如 "{2,6,8,10}"）。 |
| [GetSecondCategoryData](./getsecondcategorydata/) | 获取或设置第二类别轴值的范围。它可以是单元格范围（例如 "d1:e10"），或值序列（例如 "{2,6,8,10}"）。仅在某些系列绘制在第二坐标轴时生效。 |
| [SetSecondCategoryData](./setsecondcategorydata/) | 获取或设置第二类别轴值的范围。它可以是单元格范围（例如 "d1:e10"），或值序列（例如 "{2,6,8,10}"）。仅在某些系列绘制在第二坐标轴时生效。 |
| [SwapSeries](./swapseries/) | 直接更改两个系列的顺序。 |
| [SetSeriesNames](./setseriesnames/) | 设置图表中所有系列的名称。 |
| [AddR1C1](./addr1c1/) | 将 Series 集合添加到图表中。 |
| [Add_String_Bool](./add_string_bool/) | 将 Series 集合添加到图表中。 |
| [Add_String_Bool_Bool](./add_string_bool_bool/) | 将 Series 集合添加到图表中。 |
| [IsColorVaried](./iscolorvaried/) | 表示点的颜色是否可变。 |
| [SetIsColorVaried](./setiscolorvaried/) | 表示点的颜色是否可变。 |
| [Clear](./clear/) | 清除集合 |
| [ChangeColors](./changecolors/) | 为图表系列设置单色调色板。 |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
