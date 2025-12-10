---
title: Aspose::Cells::Drawing::ShapeCollection::AddButton method
linktitle: AddButton
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::AddButton method. Adds a Button to the worksheet in C++.'
type: docs
weight: 1800
url: /cpp/aspose.cells.drawing/shapecollection/addbutton/
---
## ShapeCollection::AddButton method


Adds a [Button](../../button/) to the worksheet.

```cpp
Button Aspose::Cells::Drawing::ShapeCollection::AddButton(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of [Button](../../button/) from its left row, in unit of pixel. |
| leftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of [Button](../../button/) from its left column, in unit of pixel. |
| height | int32_t | Represents the height of [Button](../../button/), in unit of pixel. |
| width | int32_t | Represents the width of [Button](../../button/), in unit of pixel. |

## ReturnValue

A [Button](../../button/) object.


## Examples


```cpp
    //add a button
Button button = shapes.AddButton(1, 0, 1, 0, 100, 50);
```

## See Also

* Class [Button](../../button/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
