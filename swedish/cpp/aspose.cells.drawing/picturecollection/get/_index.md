---
title: Aspose::Cells::Drawing::PictureCollection::Get method
linktitle: Get
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::PictureCollection::Get method. Gets the Picture element at the specified index in C++.'
type: docs
weight: 800
url: /sv/cpp/aspose.cells.drawing/picturecollection/get/
---
## PictureCollection::Get method


Gets the [Picture](../../picture/) element at the specified index.

```cpp
Aspose::Cells::Drawing::Picture Aspose::Cells::Drawing::PictureCollection::Get(int32_t index)
```


| Parameter | Type | Description |
| --- | --- | --- |
| index | int32_t | The zero based index of the element. |

## ReturnValue

The element at the specified index.


## Examples


```cpp
//hämta bildsamling
//PictureCollection pictures = workbook.GetWorksheets().Get(0).GetPictures();
//lägg till en bild
int picIndex = pictures.Add(1, 1, u"image.png");
//hämta bilden
Picture pic = pictures.Get(picIndex);
```

## See Also

* Class [Picture](../../picture/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [PictureCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
