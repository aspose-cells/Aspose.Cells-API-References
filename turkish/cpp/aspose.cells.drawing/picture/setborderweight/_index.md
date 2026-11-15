---
title: Aspose::Cells::Drawing::Picture::SetBorderWeight method
linktitle: SetBorderWeight
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::SetBorderWeight method. Gets or sets the weight of the border line of a picture in units of pt in C++.'
type: docs
weight: 1600
url: /tr/cpp/aspose.cells.drawing/picture/setborderweight/
---
## Picture::SetBorderWeight method


Gets or sets the weight of the border line of a picture in units of pt.

```cpp
void Aspose::Cells::Drawing::Picture::SetBorderWeight(double value)
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
pic.SetBorderLineColor(Color{ 0xff, 0xff, 0, 0 });//Red
//Resmin kenar genişliğini ayarla
if (pic.GetBorderWeight() == 3)
{
    pic.SetBorderWeight(3);
}
//Excel dosyasını kaydedin.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
