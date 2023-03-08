---
title: get_display_style方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 110
url: /zh/python-net/aspose.cells/cell/get_display_style/
is_root: false
---
##  get_display_style() {#}
获取单元格的显示样式。
如果此单元格还受到条件格式、列表对象等其他设置的影响，
那么显示样式可能与cell.GetStyle()不同。



```python
def get_display_style(self):
    ...
```




##  get_display_style(include_merged_borders) {#bool}
获取单元格的显示样式。
如果单元格是条件格式，则显示样式与 cell.GetStyle() 不同。



```python
def get_display_style(self, include_merged_borders):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| include_merged_borders | bool |指示是否检查合并单元格的边框。|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Cell](/cells/zh/python-net/aspose.cells/cell)
