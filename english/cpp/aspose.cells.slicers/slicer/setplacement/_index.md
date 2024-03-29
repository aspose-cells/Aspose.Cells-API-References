﻿---
title: Aspose::Cells::Slicers::Slicer::SetPlacement method
linktitle: SetPlacement
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Slicers::Slicer::SetPlacement method. Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet in C++.'
type: docs
weight: 1700
url: /cpp/aspose.cells.slicers/slicer/setplacement/
---
## Slicer::SetPlacement method


Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.

```cpp
void Aspose::Cells::Slicers::Slicer::SetPlacement(PlacementType value)
```


## Examples


```cpp
if (slicer.GetPlacement() != PlacementType::FreeFloating)
{
    slicer.SetPlacement(PlacementType::FreeFloating);
}
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Enum [PlacementType](../../../aspose.cells.drawing/placementtype/)
* Class [Slicer](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
