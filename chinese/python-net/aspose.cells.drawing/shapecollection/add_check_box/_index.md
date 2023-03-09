---
title: add_check_box方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 70
url: /zh/python-net/aspose.cells.drawing/shapecollection/add_check_box/
is_root: false
---
##  add_check_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
向工作表添加一个复选框。


### 返回

新的 CheckBox 对象索引。


```python
def add_check_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| upper_left_row | int |左上行索引。|
| top | int |表示复选框相对于其左行的垂直偏移量，以像素为单位。|
| upper_left_column | int |左上列索引。|
| left | int |表示文本框与其左列的水平偏移量，以像素为单位。|
| height | int |文本框的高度，以像素为单位。|
| width | int |文本框的宽度，以像素为单位。|

### 例子

```python

# add a CheckBox
checkBox = shapes.add_check_box(1, 0, 1, 0, 100, 50)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ShapeCollection](/cells/zh/python-net/aspose.cells.drawing/shapecollection)
