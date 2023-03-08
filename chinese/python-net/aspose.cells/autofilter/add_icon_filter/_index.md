---
title: add_icon_filter方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 60
url: /zh/python-net/aspose.cells/autofilter/add_icon_filter/
is_root: false
---
##  add_icon_filter(field_index, icon_set_type, icon_id) {#int-IconSetType-int}
添加图标过滤器。



```python
def add_icon_filter(self, field_index, icon_set_type, icon_id):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| field_index | int |要作为过滤器基础的字段的整数偏移量<br/>（从列表的左边开始；最左边的字段是字段 0）。|
| icon_set_type | [IconSetType](/cells/zh/python-net/aspose.cells/iconsettype) |图标集类型。|
| icon_id | int |图标标识。|
### 评论

只支持添加图标过滤器。
如果过滤器是图标过滤器，则不支持检查哪一行可见。


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [AutoFilter](/cells/zh/python-net/aspose.cells/autofilter)
