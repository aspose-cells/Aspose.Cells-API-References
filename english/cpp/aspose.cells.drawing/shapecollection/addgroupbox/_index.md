---
title: Aspose::Cells::Drawing::ShapeCollection::AddGroupBox method
linktitle: AddGroupBox
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::AddGroupBox method. Adds a GroupBox to the worksheet in C++.'
type: docs
weight: 1700
url: /cpp/aspose.cells.drawing/shapecollection/addgroupbox/
---
## ShapeCollection::AddGroupBox method


Adds a [GroupBox](../../groupbox/) to the worksheet.

```cpp
GroupBox Aspose::Cells::Drawing::ShapeCollection::AddGroupBox(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of [GroupBox](../../groupbox/) from its left row, in unit of pixel. |
| leftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of [GroupBox](../../groupbox/) from its left column, in unit of pixel. |
| height | int32_t | Represents the height of [GroupBox](../../groupbox/), in unit of pixel. |
| width | int32_t | Represents the width of [GroupBox](../../groupbox/), in unit of pixel. |

## ReturnValue

A [GroupBox](../../groupbox/) object.


## Examples


```cpp
    //add a group box
GroupBox groupBox = shapes.AddGroupBox(1, 0, 1, 0, 100, 50);
```

## See Also

* Class [GroupBox](../../groupbox/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
