---
title: Aspose::Cells::Drawing::Picture::GetImageType method
linktitle: GetImageType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetImageType method. Gets the image format of the picture in C++.'
type: docs
weight: 2900
url: /zh/cpp/aspose.cells.drawing/picture/getimagetype/
---
## Picture::GetImageType method


Gets the image format of the picture.

```cpp
Aspose::Cells::Drawing::ImageType Aspose::Cells::Drawing::Picture::GetImageType()
```


## Examples


```cpp
Aspose::Cells::Startup();
//实例化 Workbook 对象
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//插入第一张图片
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"1.png");
//获取插入的图片对象
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
if (pic1.GetImageType() == ImageType::Png)
{
    //图片的类型是 png.";
}
//插入第二张图片
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"2.jpeg");
//获取插入的图片对象
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
if (pic2.GetImageType() == ImageType::Jpeg)
{
    //图片的类型是 jpg.";
}
Aspose::Cells::Cleanup();
```

## See Also

* Enum [ImageType](../../imagetype/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
