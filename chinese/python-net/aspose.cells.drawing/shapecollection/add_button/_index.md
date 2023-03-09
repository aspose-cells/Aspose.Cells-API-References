---
title: add_button方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 60
url: /zh/python-net/aspose.cells.drawing/shapecollection/add_button/
is_root: false
---
##  add_button(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
向工作表添加一个按钮。


### 返回

一个按钮对象。


```python
def add_button(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| upper_left_row | int |左上行索引。|
| top | int |表示 Button 从其左行的垂直偏移量，以像素为单位。|
| upper_left_column | int |左上列索引。|
| left | int |表示 Button 与其左列的水平偏移量，以像素为单位。|
| height | int |表示Button的高度，单位为像素。|
| width | int |表示Button的宽度，以像素为单位。|

### 例子

```python

# add a button
button = shapes.add_button(1, 0, 1, 0, 100, 50)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ShapeCollection](/cells/zh/python-net/aspose.cells.drawing/shapecollection)
