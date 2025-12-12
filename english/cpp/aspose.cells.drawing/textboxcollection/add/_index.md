---
title: Aspose::Cells::Drawing::TextBoxCollection::Add method
linktitle: Add
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::TextBoxCollection::Add method. Adds a textbox to the collection in C++.'
type: docs
weight: 700
url: /cpp/aspose.cells.drawing/textboxcollection/add/
---
## TextBoxCollection::Add method


Adds a textbox to the collection.

```cpp
int32_t Aspose::Cells::Drawing::TextBoxCollection::Add(int32_t topRow, int32_t leftColumn, int32_t height, int32_t width)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| leftColumn | int32_t | Upper left column index. |
| height | int32_t | Height of textbox, in unit of pixel. |
| width | int32_t | Width of textbox, in unit of pixel. |

## ReturnValue

[TextBox](../../textbox/) object index.


## Examples


```cpp
    //add a TextBox
int index2 = textBoxCollection.Add(1, 1, 50, 100);
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [TextBoxCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
