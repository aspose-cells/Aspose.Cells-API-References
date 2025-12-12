---
title: Aspose::Cells::Drawing::ShapeCollection::AddShape method
linktitle: AddShape
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::AddShape method. Adds a Shape to the worksheet in C++.'
type: docs
weight: 3200
url: /cpp/aspose.cells.drawing/shapecollection/addshape/
---
## ShapeCollection::AddShape method


Adds a [Shape](../../shape/) to the worksheet.

```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::AddShape(MsoDrawingType type, int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)
```


| Parameter | Type | Description |
| --- | --- | --- |
| type | MsoDrawingType | Mso drawing type. |
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
    //Add a shape of the specified type
Shape shapeByType = shapes.AddShape(MsoDrawingType::CellsDrawing, 1, 0, 1, 0, 100, 50);
```

## See Also

* Class [Shape](../../shape/)
* Enum [MsoDrawingType](../../msodrawingtype/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
