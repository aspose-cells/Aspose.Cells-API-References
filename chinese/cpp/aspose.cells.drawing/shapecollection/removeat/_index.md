---
title: Aspose::Cells::Drawing::ShapeCollection::RemoveAt method
linktitle: RemoveAt
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::RemoveAt method. Remove the shape in C++.'
type: docs
weight: 4800
url: /zh/cpp/aspose.cells.drawing/shapecollection/removeat/
---
## ShapeCollection::RemoveAt method


Remove the shape.

```cpp
void Aspose::Cells::Drawing::ShapeCollection::RemoveAt(int32_t index)
```


| Parameter | Type | Description |
| --- | --- | --- |
| index | int32_t | The index of the shape. |


## Examples


```cpp
    //添加第一个形状
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
//添加第二个形状
shapes.AddRectangle(6, 0, 2, 0, 30, 30);

//删除
shapes.RemoveAt(0);
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
