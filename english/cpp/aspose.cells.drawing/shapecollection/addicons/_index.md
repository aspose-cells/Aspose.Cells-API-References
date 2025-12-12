---
title: Aspose::Cells::Drawing::ShapeCollection::AddIcons method
linktitle: AddIcons
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::AddIcons method. Adds svg image in C++.'
type: docs
weight: 3800
url: /cpp/aspose.cells.drawing/shapecollection/addicons/
---
## ShapeCollection::AddIcons method


Adds svg image.

```cpp
Aspose::Cells::Drawing::Picture Aspose::Cells::Drawing::ShapeCollection::AddIcons(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width, const Vector<uint8_t> &imageByteData, const Vector<uint8_t> &compatibleImageData)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of shape from its left row, in unit of pixel. |
| leftColumn | int32_t | Upper left column index. |
| left | int32_t | The horizontal offset of shape from its left column, in unit of pixel. |
| height | int32_t | The height of shape, in unit of pixel. |
| width | int32_t | The width of shape, in unit of pixel. |
| imageByteData | const Vector \<uint8_t\>\& | The image byte data. |
| compatibleImageData | const Vector \<uint8_t\>\& | Converted image data from svg in order to be compatible with Excel 2016 or lower versions. |

## ReturnValue




## Examples


```cpp
//add icon
Vector<uint8_t> imageData{ 0 };//Gets image data into 'imageData' from file(e.g image.svg . Note: You need to read the data into this variable.).
Picture picture = shapes.AddIcons(4, 0, 5, 0, -1, -1, imageData, Vector<uint8_t>(0));
```

## See Also

* Class [Picture](../../picture/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
