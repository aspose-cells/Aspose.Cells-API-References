---
title: Aspose::Cells::Drawing::PictureCollection::Get method
linktitle: Get
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::PictureCollection::Get method. Gets the Picture element at the specified index in C++.'
type: docs
weight: 700
url: /cpp/aspose.cells.drawing/picturecollection/get/
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
//get picture collection
//PictureCollection pictures = workbook.GetWorksheets().Get(0).GetPictures();
//add a picture
int picIndex = pictures.Add(1, 1, u"image.png");
//get the picture
Picture pic = pictures.Get(picIndex);
```

## See Also

* Class [Picture](../../picture/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [PictureCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
