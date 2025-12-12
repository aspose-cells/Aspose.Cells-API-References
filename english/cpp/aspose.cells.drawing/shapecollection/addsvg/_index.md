---
title: Aspose::Cells::Drawing::ShapeCollection::AddSvg method
linktitle: AddSvg
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::AddSvg method. Adds svg image in C++.'
type: docs
weight: 3700
url: /cpp/aspose.cells.drawing/shapecollection/addsvg/
---
## ShapeCollection::AddSvg method


Adds svg image.

```cpp
Aspose::Cells::Drawing::Picture Aspose::Cells::Drawing::ShapeCollection::AddSvg(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width, const Vector<uint8_t> &svgData, const Vector<uint8_t> &compatibleImageData)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of shape from its left row, in unit of pixel. |
| leftColumn | int32_t | Upper left column index. |
| left | int32_t | The horizontal offset of shape from its left column, in unit of pixel. |
| height | int32_t | The height of shape, in unit of pixel. |
| width | int32_t | The width of shape, in unit of pixel. |
| svgData | const Vector \<uint8_t\>\& | The svg image data. |
| compatibleImageData | const Vector \<uint8_t\>\& | Converted image data from svg in order to be compatible with Excel 2016 or lower versions. |

## ReturnValue




## Examples


```cpp
// add a svg
Vector<uint8_t> fs{ 0 };//Gets image data into fs from file(e.g image.svg . Note: You need to read the data into this variable.).
Picture picture = shapes.AddSvg(4, 0, 5, 0, -1, -1, fs, Vector<uint8_t>(0));
```

## See Also

* Class [Picture](../../picture/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
