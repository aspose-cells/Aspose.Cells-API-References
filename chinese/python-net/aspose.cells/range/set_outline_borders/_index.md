---
title: set_outline_borders方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 180
url: /zh/python-net/aspose.cells/range/set_outline_borders/
is_root: false
---
##  set_outline_borders(border_style, border_color) {#CellBorderType-CellsColor}
在具有相同边框样式和颜色的一系列单元格周围设置轮廓边框。



```python
def set_outline_borders(self, border_style, border_color):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| border_style | [CellBorderType](/cells/zh/python-net/aspose.cells/cellbordertype) |边框样式。|
| border_color | [CellsColor](/cells/zh/python-net/aspose.cells/cellscolor) |边框颜色。|


##  set_outline_borders(border_style, border_color) {#CellBorderType-aspose.pydrawing.Color}
在具有相同边框样式和颜色的一系列单元格周围设置轮廓边框。



```python
def set_outline_borders(self, border_style, border_color):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| border_style | [CellBorderType](/cells/zh/python-net/aspose.cells/cellbordertype) |边框样式。|
| border_color | aspose.pydrawing.Color |边框颜色。|


##  set_outline_borders(border_styles, border_colors) {#list-aspose.pydrawing.Color[]}
在一系列单元格周围设置线条边框。



```python
def set_outline_borders(self, border_styles, border_colors):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| border_styles | list |边框样式。|
| border_colors | aspose.pydrawing.Color[] |边框颜色。|
### 评论

borderStyles 和 borderStyles 的长度都必须是 4。
borderStyles和borderStyles的顺序必须是top,bottom,left,right


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Range](/cells/zh/python-net/aspose.cells/range)
