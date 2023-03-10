---
title: LoadFilter类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 1010
url: /zh/python-net/aspose.cells/loadfilter/
is_root: false
---
## LoadFilter类
表示从模板加载工作簿时提供用于加载数据的选项的筛选器。



LoadFilter 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [LoadFilter()](/cells/zh/python-net/aspose.cells/loadfilter/__init__/#) |构造一个具有默认过滤器选项 LoadDataFilterOptions.All 的 LoadFilter。|
| [LoadFilter(opts)](/cells/zh/python-net/aspose.cells/loadfilter/__init__/#LoadDataFilterOptions) |使用给定的过滤器选项构造一个 LoadFilter。|


### 特性
|属性|描述|
| :- | :- |
| [load_data_filter_options](/cells/zh/python-net/aspose.cells/loadfilter/load_data_filter_options) |用于指示应加载哪些数据的过滤器选项。|
| [sheets_in_loading_order](/cells/zh/python-net/aspose.cells/loadfilter/sheets_in_loading_order) |指定要加载的工作表（索引）和顺序。<br/>默认为null，表示以模板文件中的默认顺序加载所有图纸。<br/>如果不为 null 并且某些工作表的索引不在返回的数组中，则不会加载该工作表。|


### 方法
|方法|描述|
| :- | :- |
| [start_sheet(sheet)](/cells/zh/python-net/aspose.cells/loadfilter/start_sheet/#Worksheet) |在加载给定工作表之前准备过滤器选项。<br/>用户对 LoadFilter 的实现可以在此处更改 LoadDataFilterOptions<br/>表示如何为该工作表加载数据。|



### 评论

用户可以指定过滤器选项或实现自己的 LoadFilter 来指定如何加载数据。

### 也可以看看
* 模块 [aspose.cells](..)
