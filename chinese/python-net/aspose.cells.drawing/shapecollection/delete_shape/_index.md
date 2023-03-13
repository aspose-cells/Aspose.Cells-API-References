---
title: delete_shape方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 410
url: /zh/python-net/aspose.cells.drawing/shapecollection/delete_shape/
is_root: false
---
##  delete_shape(shape) {#Shape}
删除形状。如果形状在组中或者是评论形状，则不会被删除。



```python
def delete_shape(self, shape):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| shape | [Shape](/cells/zh/python-net/aspose.cells.drawing/shape) |  |

### 例子

```python

# add first shape
firstShape = shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
secondShape = shapes.add_rectangle(6, 0, 2, 0, 30, 30)
# del
shapes.delete_shape(firstShape)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ShapeCollection](/cells/zh/python-net/aspose.cells.drawing/shapecollection)
