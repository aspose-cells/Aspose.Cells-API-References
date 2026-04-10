---
title: Aspose::Cells::Drawing::ShapeCollection::Remove method
linktitle: Remove
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::Remove method. Remove the shape in C++.'
type: docs
weight: 4900
url: /es/cpp/aspose.cells.drawing/shapecollection/remove/
---
## ShapeCollection::Remove method


Remove the shape.

```cpp
void Aspose::Cells::Drawing::ShapeCollection::Remove(const Shape &shape)
```


| Parameter | Type | Description |
| --- | --- | --- |
| shape | const Shape\& |  |


## Examples


```cpp
    //agregar primera forma
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
//agregar segunda forma
shapes.AddRectangle(6, 0, 2, 0, 30, 30);

//obtener la forma
Shape s = shapes.Get(u"Rectangle 1");// or shapes[0];
if (!s.IsNull())
{
    //eliminar
    shapes.Remove(s);
}
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../../shape/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
