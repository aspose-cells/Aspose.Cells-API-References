﻿---
title: Aspose::Cells::Drawing::Shape::SetLeftInShape method
linktitle: SetLeftInShape
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::SetLeftInShape method. Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape in C++.'
type: docs
weight: 12500
url: /cpp/aspose.cells.drawing/shape/setleftinshape/
---
## Shape::SetLeftInShape method


Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape.

```cpp
void Aspose::Cells::Drawing::Shape::SetLeftInShape(int32_t value)
```

## Remarks


Only Applies when this shape in the group or chart.

## Examples


```cpp
if (shape.IsInGroup() && shape.GetLeftInShape() == 2000)
    shape.SetLeftInShape(4000);
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
