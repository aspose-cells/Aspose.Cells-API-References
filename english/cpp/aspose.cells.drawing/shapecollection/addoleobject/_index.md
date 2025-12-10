---
title: Aspose::Cells::Drawing::ShapeCollection::AddOleObject method
linktitle: AddOleObject
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::AddOleObject method. Adds an OleObject in C++.'
type: docs
weight: 4200
url: /cpp/aspose.cells.drawing/shapecollection/addoleobject/
---
## ShapeCollection::AddOleObject method


Adds an [OleObject](../../oleobject/).

```cpp
OleObject Aspose::Cells::Drawing::ShapeCollection::AddOleObject(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width, const Vector<uint8_t> &imageData)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t |  |
| top | int32_t |  |
| leftColumn | int32_t |  |
| left | int32_t |  |
| height | int32_t |  |
| width | int32_t |  |
| imageData | const Vector \<uint8_t\>\& |  |

## ReturnValue




## Examples


```cpp
Vector<uint8_t> imgData{ 0 };//Gets image data into 'imgData' from file(e.g image.jpg . Note: You need to read the data into this variable.).
OleObject oleObject = shapes.AddOleObject(4, 0, 5, 0, 300, 500, imgData);
```

## See Also

* Class [OleObject](../../oleobject/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
