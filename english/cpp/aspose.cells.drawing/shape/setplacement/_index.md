---
title: Aspose::Cells::Drawing::Shape::SetPlacement method
linktitle: SetPlacement
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::SetPlacement method. Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet in C++.'
type: docs
weight: 6100
url: /cpp/aspose.cells.drawing/shape/setplacement/
---
## Shape::SetPlacement method


Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.

```cpp
void Aspose::Cells::Drawing::Shape::SetPlacement(PlacementType value)
```


## Examples


```cpp
if (shape.GetPlacement() == PlacementType::Move)
    shape.SetPlacement(PlacementType::MoveAndSize);
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Enum [PlacementType](../../placementtype/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
