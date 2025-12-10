---
title: Aspose::Cells::Drawing::ShapeCollection::AddAutoShape method
linktitle: AddAutoShape
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::AddAutoShape method. Adds a AutoShape to the worksheet in C++.'
type: docs
weight: 3300
url: /cpp/aspose.cells.drawing/shapecollection/addautoshape/
---
## ShapeCollection::AddAutoShape method


Adds a AutoShape to the worksheet.

```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::AddAutoShape(AutoShapeType type, int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)
```


| Parameter | Type | Description |
| --- | --- | --- |
| type | AutoShapeType | Auto shape type. |
| topRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of [Shape](../../shape/) from its left row, in unit of pixel. |
| leftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of [Shape](../../shape/) from its left column, in unit of pixel. |
| height | int32_t | Represents the height of [Shape](../../shape/), in unit of pixel. |
| width | int32_t | Represents the width of [Shape](../../shape/), in unit of pixel. |

## ReturnValue

A [Shape](../../shape/) object.
## Remarks



The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox

## Examples


```cpp
    //Adds a AutoShape to the worksheet.
Shape autoShape = shapes.AddAutoShape(AutoShapeType::Cube, 1, 0, 1, 0, 100, 50);
```

## See Also

* Class [Shape](../../shape/)
* Enum [AutoShapeType](../../autoshapetype/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
