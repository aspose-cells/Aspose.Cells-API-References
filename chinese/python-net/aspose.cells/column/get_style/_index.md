---
title: get_style方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 30
url: /zh/python-net/aspose.cells/column/get_style/
is_root: false
---
##  get_style() {#}
获取此列的样式。



```python
def get_style(self):
    ...
```


### 评论

直接修改返回的样式对象对该列或该列中的任何单元格都没有影响。
您必须调用 [Column.apply_style(style, flag)](/cells/zh/python-net/aspose.cells/column/apply_style) 或 [Column.set_style(style)](/cells/zh/python-net/aspose.cells/column/set_style) 方法
将更改应用到此列。

列的样式是该列中的单元格将继承的样式（那些没有自定义样式设置的单元格，
例如尚未明确设置样式的现有单元格，或尚未实例化的单元格）


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Column](/cells/zh/python-net/aspose.cells/column)
