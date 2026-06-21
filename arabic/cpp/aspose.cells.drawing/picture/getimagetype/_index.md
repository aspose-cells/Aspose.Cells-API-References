---
title: Aspose::Cells::Drawing::Picture::GetImageType method
linktitle: GetImageType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetImageType method. Gets the image format of the picture in C++.'
type: docs
weight: 2900
url: /ar/cpp/aspose.cells.drawing/picture/getimagetype/
---
## Picture::GetImageType method


Gets the image format of the picture.

```cpp
Aspose::Cells::Drawing::ImageType Aspose::Cells::Drawing::Picture::GetImageType()
```


## Examples


```cpp
Aspose::Cells::Startup();
//إنشاء كائن Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//إدراج الصورة الأولى
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"1.png");
//احصل على كائن الصورة المُدرَج
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
if (pic1.GetImageType() == ImageType::Png)
{
    //نوع الصورة هو png.";
}
//إدراج الصورة الثانية
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"2.jpeg");
//احصل على كائن الصورة المُدرَج
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
if (pic2.GetImageType() == ImageType::Jpeg)
{
    //نوع الصورة هو jpg.";
}
Aspose::Cells::Cleanup();
```

## See Also

* Enum [ImageType](../../imagetype/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
