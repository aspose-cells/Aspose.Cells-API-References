---
title: "LoadFilter 类"
linktitle: "LoadFilter"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "LoadFilter 类。封装在 Go 中表示 loadfilter 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/loadfilter/
---

## LoadFilter class

表示在从模板加载工作簿时提供加载数据选项的过滤器。

```go

type LoadFilter struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewLoadFilter](./newloadfilter/) | 使用默认过滤选项 LoadDataFilterOptions::All 构造一个 LoadFilter。 |
| [NewLoadFilter_LoadDataFilterOptions](./newloadfilter_loaddatafilteroptions/) | 使用给定的过滤选项构造一个 LoadFilter。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetLoadDataFilterOptions](./getloaddatafilteroptions/) | 获取过滤选项，以指示应加载哪些数据。 |
| [SetLoadDataFilterOptions](./setloaddatafilteroptions/) | 设置过滤选项，以指示应加载哪些数据。 |
| [GetSheetsInLoadingOrder](./getsheetsinloadingorder/) | 指定要加载的工作表（索引）及其顺序。默认值为 null，表示加载模板文件中按默认顺序的所有工作表。如果不为 null 且某些工作表的索引不在返回的数组中，则该工作表将不会被加载。 |
| [StartSheet](./startsheet/) | 在加载给定工作表之前准备过滤选项。用户对 LoadFilter 的实现可以更改此处的 LoadDataFilterOptions，以指示如何加载该工作表的数据。 |
