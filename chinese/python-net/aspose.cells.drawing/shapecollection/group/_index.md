---
title: group方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 420
url: /zh/python-net/aspose.cells.drawing/shapecollection/group/
is_root: false
---
##  group(group_items) {#list}
对形状进行分组。


### 返回

返回 group 形状。


```python
def group(self, group_items):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| group_items | list |组项目。|
### 评论

groupItems 中的形状不应分组。
该形状必须在此 Shapes 集合中。
### 例子

```python

# add first shape
shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
shapes.add_rectangle(6, 0, 2, 0, 30, 30)
shapesArr = [shapes[0], shapes[1]]
groupShape = shapes.group(shapesArr)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ShapeCollection](/cells/zh/python-net/aspose.cells.drawing/shapecollection)
