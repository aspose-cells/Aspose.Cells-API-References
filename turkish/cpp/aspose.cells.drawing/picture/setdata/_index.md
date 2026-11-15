---
title: Aspose::Cells::Drawing::Picture::SetData method
linktitle: SetData
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::SetData method. Gets the data of the picture in C++.'
type: docs
weight: 1800
url: /tr/cpp/aspose.cells.drawing/picture/setdata/
---
## Picture::SetData method


Gets the data of the picture.

```cpp
void Aspose::Cells::Drawing::Picture::SetData(const Vector<uint8_t> &value)
```


## Examples


```cpp
Aspose::Cells::Startup();
//Bir Workbook nesnesi oluşturuluyor
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//ilk resmi ekle
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"example1.png");
//Eklenen resim nesnesini al
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
//ikinci resmi ekle
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"example2.jpeg");
//Eklenen resim nesnesini al
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
//İlk görüntünün bayt verisini ikinci görüntüye ata
pic2.SetData(pic1.GetData());
//Excel dosyasını kaydedin.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
