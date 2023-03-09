---
title: add_filter方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 40
url: /zh/python-net/aspose.cells/autofilter/add_filter/
is_root: false
---
##  add_filter(field_index, criteria) {#int-str}
为过滤列添加过滤器。



```python
def add_filter(self, field_index, criteria):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| field_index | int |要作为过滤器基础的字段的整数偏移量<br/>（从列表的左边开始；最左边的字段是字段 0）。|
| criteria | str |指定的条件（字符串；例如“101”）。<br/>它只能为 null 或者是此列中单元格的值之一。|
### 评论

MS Excel 2007 支持在过滤列中进行多项选择。


### 也可以看看

* 模块 [aspose.cells](../../)
* 类 [AutoFilter](/cells/zh/python-net/aspose.cells/autofilter)
