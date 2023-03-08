---
title: remove_filter方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 160
url: /zh/python-net/aspose.cells/autofilter/remove_filter/
is_root: false
---
##  remove_filter(field_index) {#int}
删除特定过滤器。



```python
def remove_filter(self, field_index):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| field_index | int |具体过滤指标|


##  remove_filter(field_index, criteria) {#int-str}
删除筛选器列的筛选器。



```python
def remove_filter(self, field_index, criteria):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| field_index | int |要作为过滤器基础的字段的整数偏移量<br/>（从列表的左边开始；最左边的字段是字段 0）。|
| criteria | str |指定的条件（字符串；例如“101”）。<br/>它只能为 null 或此列中的单元格值之一。|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [AutoFilter](/cells/zh/python-net/aspose.cells/autofilter)
