---
title: Aspose::Cells::Drawing::ShapeCollection::AddListBox method
linktitle: AddListBox
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::AddListBox method. Adds a ListBox to the worksheet in C++.'
type: docs
weight: 1500
url: /cpp/aspose.cells.drawing/shapecollection/addlistbox/
---
## ShapeCollection::AddListBox method


Adds a [ListBox](../../listbox/) to the worksheet.

```cpp
ListBox Aspose::Cells::Drawing::ShapeCollection::AddListBox(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of [ListBox](../../listbox/) from its left row, in unit of pixel. |
| leftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of [ListBox](../../listbox/) from its left column, in unit of pixel. |
| height | int32_t | Represents the height of [ListBox](../../listbox/), in unit of pixel. |
| width | int32_t | Represents the width of [ListBox](../../listbox/), in unit of pixel. |

## ReturnValue

A [ListBox](../../listbox/) object.


## Examples


```cpp
    //add a list box
ListBox listBox = shapes.AddListBox(1, 0, 1, 0, 100, 50);
```

## See Also

* Class [ListBox](../../listbox/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
