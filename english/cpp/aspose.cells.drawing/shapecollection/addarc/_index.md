---
title: Aspose::Cells::Drawing::ShapeCollection::AddArc method
linktitle: AddArc
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::AddArc method. Adds a ArcShape to the worksheet in C++.'
type: docs
weight: 3100
url: /cpp/aspose.cells.drawing/shapecollection/addarc/
---
## ShapeCollection::AddArc method


Adds a [ArcShape](../../arcshape/) to the worksheet.

```cpp
ArcShape Aspose::Cells::Drawing::ShapeCollection::AddArc(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of [ArcShape](../../arcshape/) from its left row, in unit of pixel. |
| leftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of [ArcShape](../../arcshape/) from its left column, in unit of pixel. |
| height | int32_t | Represents the height of [ArcShape](../../arcshape/), in unit of pixel. |
| width | int32_t | Represents the width of [ArcShape](../../arcshape/), in unit of pixel. |

## ReturnValue

A [ArcShape](../../arcshape/) object.


## Examples


```cpp
    //add a arc
ArcShape arcShape = shapes.AddArc(1, 0, 1, 0, 100, 50);
```

## See Also

* Class [ArcShape](../../arcshape/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
