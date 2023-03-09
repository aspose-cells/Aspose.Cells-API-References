---
title: subtotal方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 920
url: /zh/python-net/aspose.cells/cells/subtotal/
is_root: false
---
##  subtotal(ca, group_by, function, total_list) {#CellArea-int-ConsolidationFunction-list}
创建范围的小计。



```python
def subtotal(self, ca, group_by, function, total_list):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| ca | [CellArea](/cells/zh/python-net/aspose.cells/cellarea) |范围|
| group_by | int |分组依据的字段，作为从零开始的整数偏移量|
| function | [ConsolidationFunction](/cells/zh/python-net/aspose.cells/consolidationfunction) |小计函数。|
| total_list | list |从零开始的字段偏移量的数组，指示要添加小计的字段。|


##  subtotal(ca, group_by, function, total_list, replace, page_breaks, summary_below_data) {#CellArea-int-ConsolidationFunction-list-bool-bool-bool}
创建范围的小计。



```python
def subtotal(self, ca, group_by, function, total_list, replace, page_breaks, summary_below_data):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| ca | [CellArea](/cells/zh/python-net/aspose.cells/cellarea) |范围|
| group_by | int |分组依据的字段，作为从零开始的整数偏移量|
| function | [ConsolidationFunction](/cells/zh/python-net/aspose.cells/consolidationfunction) |小计函数。|
| total_list | list |从零开始的字段偏移量的数组，指示要添加小计的字段。|
| replace | bool |指示是否替换当前小计|
| page_breaks | bool |表示组间是否加分页符|
| summary_below_data | bool |指示是否在数据下方添加摘要。|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Cells](/cells/zh/python-net/aspose.cells/cells)
