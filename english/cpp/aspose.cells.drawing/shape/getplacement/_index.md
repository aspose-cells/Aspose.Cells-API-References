---
title: Aspose::Cells::Drawing::Shape::GetPlacement method
linktitle: GetPlacement
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::GetPlacement method. Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet in C++.'
type: docs
weight: 5800
url: /cpp/aspose.cells.drawing/shape/getplacement/
---
## Shape::GetPlacement method


Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.

```cpp
PlacementType Aspose::Cells::Drawing::Shape::GetPlacement()
```


## Examples


```cpp
if (shape.GetPlacement() == PlacementType::Move)
    shape.SetPlacement(PlacementType::MoveAndSize);
```

## See Also

* Enum [PlacementType](../../placementtype/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
