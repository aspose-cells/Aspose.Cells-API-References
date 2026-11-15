---
title: Aspose::Cells::Drawing::Picture::GetOriginalWidthInch method
linktitle: GetOriginalWidthInch
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetOriginalWidthInch method. Gets the original width of picture, in unit of inches in C++.'
type: docs
weight: 3500
url: /tr/cpp/aspose.cells.drawing/picture/getoriginalwidthinch/
---
## Picture::GetOriginalWidthInch method


Gets the original width of picture, in unit of inches.

```cpp
double Aspose::Cells::Drawing::Picture::GetOriginalWidthInch()
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
//Resmin orijinal genişliğini alır.
double picWidthInch = pic.GetOriginalWidthInch();
//Excel dosyasını kaydedin.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
