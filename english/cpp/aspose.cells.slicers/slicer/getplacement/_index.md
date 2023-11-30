---
title: Aspose::Cells::Slicers::Slicer::GetPlacement method
linktitle: GetPlacement
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Slicers::Slicer::GetPlacement method. Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet in C++.'
type: docs
weight: 1600
url: /cpp/aspose.cells.slicers/slicer/getplacement/
---
## Slicer::GetPlacement method


Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.

```cpp
PlacementType Aspose::Cells::Slicers::Slicer::GetPlacement()
```


## Examples


```cpp
if (slicer.GetPlacement() != PlacementType::FreeFloating)
{
    slicer.SetPlacement(PlacementType::FreeFloating);
}
```

## See Also

* Enum [PlacementType](../../../aspose.cells.drawing/placementtype/)
* Class [Slicer](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
