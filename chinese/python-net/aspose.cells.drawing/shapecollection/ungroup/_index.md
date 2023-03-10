---
title: ungroup方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 450
url: /zh/python-net/aspose.cells.drawing/shapecollection/ungroup/
is_root: false
---
##  ungroup(group) {#GroupShape}
取消组合形状项目。



```python
def ungroup(self, group):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| group | [GroupShape](/cells/zh/python-net/aspose.cells.drawing/groupshape) |群形。|
### 评论

如果组形状被另一个组形状分组，则什么也不会做。
### 例子


```python

# add first shape
shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
shapes.add_rectangle(6, 0, 2, 0, 30, 30)
# group
shapesArr = [shapes[0], shapes[1]]
groupShape = shapes.group(shapesArr)
# ungroup
shapes.ungroup(groupShape)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ShapeCollection](/cells/zh/python-net/aspose.cells.drawing/shapecollection)
