---
title: add_list_box方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 170
url: /zh/python-net/aspose.cells.drawing/shapecollection/add_list_box/
is_root: false
---
##  add_list_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
将 ListBox 添加到工作表。


### 返回

一个列表框对象。


```python
def add_list_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| upper_left_row | int |左上行索引。|
| top | int |表示 ListBox 与其左行的垂直偏移量，以像素为单位。|
| upper_left_column | int |左上列索引。|
| left | int |表示 ListBox 与其左列的水平偏移量，以像素为单位。|
| height | int |表示ListBox的高度，单位为像素。|
| width | int |表示ListBox的宽度，以像素为单位。|

### 例子

```python

# add a list box
listBox = shapes.add_list_box(1, 0, 1, 0, 100, 50)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ShapeCollection](/cells/zh/python-net/aspose.cells.drawing/shapecollection)
