---
title: Aspose::Cells::Drawing::Picture::GetImageType method
linktitle: GetImageType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetImageType method. Gets the image format of the picture in C++.'
type: docs
weight: 2900
url: /de/cpp/aspose.cells.drawing/picture/getimagetype/
---
## Picture::GetImageType method


Gets the image format of the picture.

```cpp
Aspose::Cells::Drawing::ImageType Aspose::Cells::Drawing::Picture::GetImageType()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Instanziieren eines Workbook-Objekts
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//erstes Bild einfügen
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"1.png");
//Das eingefügte Bildobjekt abrufen
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
if (pic1.GetImageType() == ImageType::Png)
{
    //Der Bildtyp ist png.";
}
//zweites Bild einfügen
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"2.jpeg");
//Das eingefügte Bildobjekt abrufen
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
if (pic2.GetImageType() == ImageType::Jpeg)
{
    //Der Bildtyp ist jpg.";
}
Aspose::Cells::Cleanup();
```

## See Also

* Enum [ImageType](../../imagetype/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
