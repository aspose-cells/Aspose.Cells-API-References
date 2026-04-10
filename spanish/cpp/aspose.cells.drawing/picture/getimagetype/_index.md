---
title: Aspose::Cells::Drawing::Picture::GetImageType method
linktitle: GetImageType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetImageType method. Gets the image format of the picture in C++.'
type: docs
weight: 2900
url: /es/cpp/aspose.cells.drawing/picture/getimagetype/
---
## Picture::GetImageType method


Gets the image format of the picture.

```cpp
Aspose::Cells::Drawing::ImageType Aspose::Cells::Drawing::Picture::GetImageType()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Instanciando un objeto Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//insertar la primera imagen
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"1.png");
//Obtener el objeto de imagen insertado
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
if (pic1.GetImageType() == ImageType::Png)
{
    //El tipo de la imagen es png.";
}
//insertar la segunda imagen
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"2.jpeg");
//Obtener el objeto de imagen insertado
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
if (pic2.GetImageType() == ImageType::Jpeg)
{
    //El tipo de la imagen es jpg.";
}
Aspose::Cells::Cleanup();
```

## See Also

* Enum [ImageType](../../imagetype/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
