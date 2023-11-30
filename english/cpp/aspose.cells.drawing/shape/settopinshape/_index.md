---
title: Aspose::Cells::Drawing::Shape::SetTopInShape method
linktitle: SetTopInShape
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::SetTopInShape method. Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape in C++.'
type: docs
weight: 12100
url: /cpp/aspose.cells.drawing/shape/settopinshape/
---
## Shape::SetTopInShape method


Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.

```cpp
void Aspose::Cells::Drawing::Shape::SetTopInShape(int32_t value)
```

## Remarks


Only Applies when this shape in the group or chart.

## Examples


```cpp
if (shape.IsInGroup() && shape.GetTopInShape() == 8000)
    shape.SetTopInShape(4000);
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
