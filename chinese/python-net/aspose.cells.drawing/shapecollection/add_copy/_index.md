---
title: add_copy方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 90
url: /zh/python-net/aspose.cells.drawing/shapecollection/add_copy/
is_root: false
---
##  add_copy(source_shape, upper_left_row, top, upper_left_column, left) {#Shape-int-int-int-int}
添加形状并将其复制到工作表。


### 返回

新的形状对象索引。


```python
def add_copy(self, source_shape, upper_left_row, top, upper_left_column, left):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| source_shape | [Shape](/cells/zh/python-net/aspose.cells.drawing/shape) |源形状。|
| upper_left_row | int |左上行索引。|
| top | int |表示复选框相对于其左行的垂直偏移量，以像素为单位。|
| upper_left_column | int |左上列索引。|
| left | int |表示文本框与其左列的水平偏移量，以像素为单位。|

### 例子

```python

# add a shape
rectangle = shapes.add_rectangle(2, 0, 2, 0, 130, 130)
# copy
shapes.add_copy(rectangle, 7, 0, 7, 0)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ShapeCollection](/cells/zh/python-net/aspose.cells.drawing/shapecollection)
