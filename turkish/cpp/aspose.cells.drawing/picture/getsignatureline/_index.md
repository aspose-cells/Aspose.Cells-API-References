---
title: Aspose::Cells::Drawing::Picture::GetSignatureLine method
linktitle: GetSignatureLine
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetSignatureLine method. Gets and sets the signature line in C++.'
type: docs
weight: 3600
url: /tr/cpp/aspose.cells.drawing/picture/getsignatureline/
---
## Picture::GetSignatureLine method


Gets and sets the signature line.

```cpp
SignatureLine Aspose::Cells::Drawing::Picture::GetSignatureLine()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Bir Workbook nesnesi oluşturuluyor
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Çalışma sayfasında satır ve sütun indeksleri 1 olan hücrenin konumuna bir resim ekleniyor. Bu "B2" hücresidir.
int imgIndex = worksheet.GetPictures().Add(1, 1, Vector<uint8_t>(0));
//Eklenen resim nesnesini al
Picture pic = worksheet.GetPictures().Get(imgIndex);
// İmza satırı nesnesi oluştur
SignatureLine s;
s.SetSigner(u"Simon Zhao");
s.SetTitle(u"Development Lead");
s.SetEmail(u"Simon.Zhao@aspose.com");
// İmza satırı nesnesini Resme ata.
pic.SetSignatureLine(s);

SignatureLine s2 = pic.GetSignatureLine();
if (s2.GetSigner() == s.GetSigner())
{
    //İstediğini yap
}
//Excel dosyasını kaydedin.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [SignatureLine](../../signatureline/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
