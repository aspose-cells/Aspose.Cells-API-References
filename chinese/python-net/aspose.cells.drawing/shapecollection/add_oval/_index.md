---
title: add_oval方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 200
url: /zh/python-net/aspose.cells.drawing/shapecollection/add_oval/
is_root: false
---
##  add_oval(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
向工作表添加椭圆。


### 返回

椭圆形物体。


```python
def add_oval(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| upper_left_row | int |左上行索引。|
| top | int |表示 Oval 从其左行的垂直偏移量，以像素为单位。|
| upper_left_column | int |左上列索引。|
| left | int |表示 Oval 从其左列的水平偏移量，以像素为单位。|
| height | int |表示 Oval 的高度，单位为像素。|
| width | int |表示 Oval 的宽度，以像素为单位。|

### 例子

```python

# add a oval
oval = shapes.add_oval(1, 0, 1, 0, 50, 50)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ShapeCollection](/cells/zh/python-net/aspose.cells.drawing/shapecollection)
