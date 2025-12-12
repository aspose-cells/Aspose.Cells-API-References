---
title: Aspose::Cells::Drawing::ShapeCollection::AddScrollBar method
linktitle: AddScrollBar
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::AddScrollBar method. Adds a ScrollBar to the worksheet in C++.'
type: docs
weight: 1300
url: /cpp/aspose.cells.drawing/shapecollection/addscrollbar/
---
## ShapeCollection::AddScrollBar method


Adds a [ScrollBar](../../scrollbar/) to the worksheet.

```cpp
ScrollBar Aspose::Cells::Drawing::ShapeCollection::AddScrollBar(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of [ScrollBar](../../scrollbar/) from its left row, in unit of pixel. |
| leftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of [ScrollBar](../../scrollbar/) from its left column, in unit of pixel. |
| height | int32_t | Represents the height of [ScrollBar](../../scrollbar/), in unit of pixel. |
| width | int32_t | Represents the width of [ScrollBar](../../scrollbar/), in unit of pixel. |

## ReturnValue

A [ScrollBar](../../scrollbar/) object.


## Examples


```cpp
    //add a scroll bar
ScrollBar scrollBar = shapes.AddScrollBar(1, 0, 1, 0, 100, 20);
```

## See Also

* Class [ScrollBar](../../scrollbar/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
