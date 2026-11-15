---
title: Aspose::Cells::Drawing::Picture::Copy method
linktitle: Copy
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::Copy method. Copy the picture in C++.'
type: docs
weight: 600
url: /tr/cpp/aspose.cells.drawing/picture/copy/
---
## Picture::Copy method


Copy the picture.

```cpp
void Aspose::Cells::Drawing::Picture::Copy(const Aspose::Cells::Drawing::Picture &source, const CopyOptions &options)
```


| Parameter | Type | Description |
| --- | --- | --- |
| source | const Aspose::Cells::Drawing::Picture\& | The source picture. |
| options | const CopyOptions\& | The copy options. |


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
//ikinci resmi ekle
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"2.jpeg");
//Eklenen resim nesnesini al
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
//Resim 1'i resim 2'ye kopyala. Üst üste bindirilmiş iki resim 1 nesnesi elde edeceksiniz.
CopyOptions opt;
pic2.Copy(pic1, opt);
//Excel dosyasını kaydedin.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Class [CopyOptions](../../../aspose.cells/copyoptions/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
