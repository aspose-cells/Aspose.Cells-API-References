---
title: Aspose::Cells::Drawing::Shape::GetHeightInShape method
linktitle: GetHeightInShape
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::GetHeightInShape method. Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape in C++.'
type: docs
weight: 12800
url: /cpp/aspose.cells.drawing/shape/getheightinshape/
---
## Shape::GetHeightInShape method


Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape..

```cpp
int32_t Aspose::Cells::Drawing::Shape::GetHeightInShape()
```

## Remarks


Only Applies when this shape in the group or chart.

## Examples


```cpp
if (shape.IsInGroup() && shape.GetHeightInShape() == 4000)
    shape.SetHeightInShape(2000);
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
