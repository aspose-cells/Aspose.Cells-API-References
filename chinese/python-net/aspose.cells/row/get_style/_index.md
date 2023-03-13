---
title: get_style方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 70
url: /zh/python-net/aspose.cells/row/get_style/
is_root: false
---
##  get_style() {#}
获取此行的样式。



```python
def get_style(self):
    ...
```


### 评论

直接修改返回的样式对象对该行或该行中的任何单元格都没有影响。
您必须调用 [Row.apply_style(style, flag)](/cells/zh/python-net/aspose.cells/row/apply_style) 或 [Row.set_style(style)](/cells/zh/python-net/aspose.cells/row/set_style) 方法
将更改应用于此行。

行的样式是该行的单元格将继承的样式（那些没有自定义样式设置的单元格，
例如尚未明确设置样式的现有单元格，或尚未实例化的单元格）


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Row](/cells/zh/python-net/aspose.cells/row)
