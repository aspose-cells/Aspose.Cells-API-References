---
title: add_combo_box方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 80
url: /zh/python-net/aspose.cells.drawing/shapecollection/add_combo_box/
is_root: false
---
##  add_combo_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
将 ComboBox 添加到工作表。


### 返回

组合框对象。


```python
def add_combo_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| upper_left_row | int |左上行索引。|
| top | int |表示 ComboBox 与其左行的垂直偏移量，以像素为单位。|
| upper_left_column | int |左上列索引。|
| left | int |表示 ComboBox 与其左列的水平偏移量，以像素为单位。|
| height | int |表示 ComboBox 的高度，以像素为单位。|
| width | int |表示 ComboBox 的宽度，以像素为单位。|

### 例子

```python

# add a combo box
comboBox = shapes.add_combo_box(1, 0, 1, 0, 100, 50)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ShapeCollection](/cells/zh/python-net/aspose.cells.drawing/shapecollection)
