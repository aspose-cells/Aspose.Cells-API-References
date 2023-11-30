---
title: Aspose::Cells::Drawing::ShapeCollection::AddCopy method
linktitle: AddCopy
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::AddCopy method. Adds and copy a shape to the worksheet in C++.'
type: docs
weight: 700
url: /cpp/aspose.cells.drawing/shapecollection/addcopy/
---
## ShapeCollection::AddCopy method


Adds and copy a shape to the worksheet.

```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::AddCopy(const Shape &sourceShape, int32_t upperLeftRow, int32_t top, int32_t upperLeftColumn, int32_t left)
```


| Parameter | Type | Description |
| --- | --- | --- |
| sourceShape | const Shape\& | Source shape. |
| upperLeftRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of checkbox from its left row, in unit of pixel. |
| upperLeftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of textbox from its left column, in unit of pixel. |

## ReturnValue

The new shape object index.


## Examples


```cpp
    //add a shape
RectangleShape rectangle = shapes.AddRectangle(2, 0, 2, 0, 130, 130);
//copy
shapes.AddCopy(rectangle, 7, 0, 7, 0);
```

## See Also

* Class [Shape](../../shape/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
