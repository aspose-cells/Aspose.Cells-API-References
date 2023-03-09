---
title: get_range_by_name方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 120
url: /zh/python-net/aspose.cells/worksheetcollection/get_range_by_name/
is_root: false
---
##  get_range_by_name(range_name) {#str}
通过预定义名称获取 Range 对象。


### 返回

范围对象。


如果命名范围不存在，则返回 null。


```python
def get_range_by_name(self, range_name):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| range_name | str |范围名称。|


##  get_range_by_name(range_name, current_sheet_index, include_table) {#str-int-bool}
通过预定义名称或表名获取 [Range](/cells/zh/python-net/aspose.cells/range)


### 返回




```python
def get_range_by_name(self, range_name, current_sheet_index, include_table):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| range_name | str |范围的名称或表的名称。|
| current_sheet_index | int |工作表索引。-1 代表全局。|
| include_table | bool |表示是否检查所有表。|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Range](/cells/zh/python-net/aspose.cells/range)
* 类 [WorksheetCollection](/cells/zh/python-net/aspose.cells/worksheetcollection)
