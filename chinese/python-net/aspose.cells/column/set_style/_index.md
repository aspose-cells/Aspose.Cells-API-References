---
title: set_style方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 40
url: /zh/python-net/aspose.cells/column/set_style/
is_root: false
---
##  set_style(style) {#Style}
设置此列的样式。



```python
def set_style(self, style):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| style | [Style](/cells/zh/python-net/aspose.cells/style) |用作此列中单元格的默认样式的样式。|
### 评论

此方法仅将给定样式设置为该列的默认样式，
无需更改此列中现有单元格的样式设置。
要同时将现有单元格的样式设置更新为指定样式，
请使用 [Column.apply_style(style, flag)](/cells/zh/python-net/aspose.cells/column/apply_style)


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Column](/cells/zh/python-net/aspose.cells/column)
