---
title: Aspose::Cells::Drawing::ShapeCollection::DeleteShape method
linktitle: DeleteShape
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::DeleteShape method. Delete a shape. If the shape is in the group or is a comment shape, it will not be deleted in C++.'
type: docs
weight: 4600
url: /ar/cpp/aspose.cells.drawing/shapecollection/deleteshape/
---
## ShapeCollection::DeleteShape method


Delete a shape. If the shape is in the group or is a comment shape, it will not be deleted.

```cpp
void Aspose::Cells::Drawing::ShapeCollection::DeleteShape(const Shape &shape)
```


| Parameter | Type | Description |
| --- | --- | --- |
| shape | const Shape\& |  |


## Examples


```cpp
    //أضف الشكل الأول
Shape firstShape = shapes.AddRectangle(2, 0, 2, 0, 50, 50);
//أضف الشكل الثاني
Shape secondShape = shapes.AddRectangle(6, 0, 2, 0, 30, 30);
//حذف
shapes.DeleteShape(firstShape);
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../../shape/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
