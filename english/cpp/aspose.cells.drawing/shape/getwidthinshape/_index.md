---
title: Aspose::Cells::Drawing::Shape::GetWidthInShape method
linktitle: GetWidthInShape
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::GetWidthInShape method. Represents the width of the shape, in unit of 1/4000 of the parent shape in C++.'
type: docs
weight: 12400
url: /cpp/aspose.cells.drawing/shape/getwidthinshape/
---
## Shape::GetWidthInShape method


Represents the width of the shape, in unit of 1/4000 of the parent shape.

```cpp
int32_t Aspose::Cells::Drawing::Shape::GetWidthInShape()
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
