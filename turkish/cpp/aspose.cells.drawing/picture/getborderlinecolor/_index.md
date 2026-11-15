---
title: Aspose::Cells::Drawing::Picture::GetBorderLineColor method
linktitle: GetBorderLineColor
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetBorderLineColor method. Represents the Color of the border line of a picture in C++.'
type: docs
weight: 1300
url: /tr/cpp/aspose.cells.drawing/picture/getborderlinecolor/
---
## Picture::GetBorderLineColor method


Represents the [Color](../../../aspose.cells/color/) of the border line of a picture.

```cpp
Aspose::Cells::Color Aspose::Cells::Drawing::Picture::GetBorderLineColor()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Bir Workbook nesnesi oluşturuluyor
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Çalışma sayfasında satır ve sütun indeksleri 1 olan hücrenin konumuna bir resim ekleniyor. Bu "B2" hücresidir.
int imgIndex = worksheet.GetPictures().Add(1, 1, u"example.jpeg");
//Eklenen resim nesnesini al
Picture pic = worksheet.GetPictures().Get(imgIndex);
//Resmin kenar rengini ayarla
if (pic.GetBorderLineColor() == Color{ 0xff, 0, 0, 0xff })//Blue
{
    pic.SetBorderLineColor(Color{ 0xff, 0xff, 0, 0 });//Red
}
//Excel dosyasını kaydedin.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
