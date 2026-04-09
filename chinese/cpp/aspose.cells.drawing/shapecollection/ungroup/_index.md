---
title: Aspose::Cells::Drawing::ShapeCollection::Ungroup method
linktitle: Ungroup
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::Ungroup method. Ungroups the shape items in C++.'
type: docs
weight: 4700
url: /zh/cpp/aspose.cells.drawing/shapecollection/ungroup/
---
## ShapeCollection::Ungroup method


Ungroups the shape items.

```cpp
void Aspose::Cells::Drawing::ShapeCollection::Ungroup(const GroupShape &group)
```


| Parameter | Type | Description |
| --- | --- | --- |
| group | const GroupShape\& | The group shape. |
## Remarks



If the group shape is grouped by another group shape,nothing will be done.

## Examples


```cpp
    //添加第一个形状
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
//添加第二个形状
shapes.AddRectangle(6, 0, 2, 0, 30, 30);

//组合
Vector<Shape> shapesArr{ shapes.Get(0), shapes.Get(1) };
GroupShape groupShape = shapes.Group(shapesArr);

//取消组合
shapes.Ungroup(groupShape);
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [GroupShape](../../groupshape/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
