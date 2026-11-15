---
title: Aspose::Cells::Drawing::Picture::GetImageType method
linktitle: GetImageType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetImageType method. Gets the image format of the picture in C++.'
type: docs
weight: 3100
url: /tr/cpp/aspose.cells.drawing/picture/getimagetype/
---
## Picture::GetImageType method


Gets the image format of the picture.

```cpp
Aspose::Cells::Drawing::ImageType Aspose::Cells::Drawing::Picture::GetImageType()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Bir Workbook nesnesi oluşturuluyor
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//ilk resmi ekle
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"1.png");
//Eklenen resim nesnesini al
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
if (pic1.GetImageType() == ImageType::Png)
{
    //Resmin türü png.";
}
//ikinci resmi ekle
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"2.jpeg");
//Eklenen resim nesnesini al
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
if (pic2.GetImageType() == ImageType::Jpeg)
{
    //Resmin türü jpg.";
}
Aspose::Cells::Cleanup();
```

## See Also

* Enum [ImageType](../../imagetype/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
