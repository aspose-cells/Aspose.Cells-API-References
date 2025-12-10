---
title: Aspose::Cells::Drawing::ShapeCollection::AddOval method
linktitle: AddOval
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::AddOval method. Adds a Oval to the worksheet in C++.'
type: docs
weight: 2600
url: /cpp/aspose.cells.drawing/shapecollection/addoval/
---
## ShapeCollection::AddOval method


Adds a [Oval](../../oval/) to the worksheet.

```cpp
Oval Aspose::Cells::Drawing::ShapeCollection::AddOval(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of [Oval](../../oval/) from its left row, in unit of pixel. |
| leftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of [Oval](../../oval/) from its left column, in unit of pixel. |
| height | int32_t | Represents the height of [Oval](../../oval/), in unit of pixel. |
| width | int32_t | Represents the width of [Oval](../../oval/), in unit of pixel. |

## ReturnValue

A [Oval](../../oval/) object.


## Examples


```cpp
    //add a oval
Oval oval = shapes.AddOval(1, 0, 1, 0, 50, 50);
```

## See Also

* Class [Oval](../../oval/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
