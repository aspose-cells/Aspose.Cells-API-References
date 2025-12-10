---
title: Aspose::Cells::Drawing::ShapeCollection::AddLabel method
linktitle: AddLabel
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::AddLabel method. Adds a Label to the worksheet in C++.'
type: docs
weight: 1900
url: /cpp/aspose.cells.drawing/shapecollection/addlabel/
---
## ShapeCollection::AddLabel method


Adds a [Label](../../label/) to the worksheet.

```cpp
Label Aspose::Cells::Drawing::ShapeCollection::AddLabel(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of [Label](../../label/) from its left row, in unit of pixel. |
| leftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of [Label](../../label/) from its left column, in unit of pixel. |
| height | int32_t | Represents the height of [Label](../../label/), in unit of pixel. |
| width | int32_t | Represents the width of [Label](../../label/), in unit of pixel. |

## ReturnValue

A [Label](../../label/) object.


## Examples


```cpp
    //add a label
Label label = shapes.AddLabel(1, 0, 1, 0, 100, 50);
```

## See Also

* Class [Label](../../label/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
