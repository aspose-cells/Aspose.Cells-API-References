---
title: Aspose::Cells::Drawing::Shape::SetWidthInShape method
linktitle: SetWidthInShape
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::SetWidthInShape method. Represents the width of the shape, in unit of 1/4000 of the parent shape in C++.'
type: docs
weight: 12700
url: /cpp/aspose.cells.drawing/shape/setwidthinshape/
---
## Shape::SetWidthInShape method


Represents the width of the shape, in unit of 1/4000 of the parent shape.

```cpp
void Aspose::Cells::Drawing::Shape::SetWidthInShape(int32_t value)
```

## Remarks


Only Applies when this shape in the group or chart.

## Examples


```cpp
if (shape.IsInGroup() && shape.GetWidthInShape() == 2000)
    shape.SetWidthInShape(4000);
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
