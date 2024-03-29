---
title: Copy
second_title: Aspose.Cells for .NET API Referansı
description: Resmi kopyalayın.
type: docs
weight: 180
url: /tr/net/aspose.cells.drawing/picture/copy/
---
## Picture.Copy method

Resmi kopyalayın.

```csharp
public void Copy(Picture source, CopyOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| source | Picture | Kaynak resim. |
| options | CopyOptions | Kopyalama seçenekleri. |

### Örnekler

```csharp

[C#]
//Bir Çalışma Kitabı nesnesini başlatma
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
//ilk resmi ekle
int imgIndex1 = worksheet.Pictures.Add(1, 1, "1.png");
// Eklenen resim nesnesini al
Picture pic1 = worksheet.Pictures[imgIndex1];
//ikinci resmi ekle
int imgIndex2 = worksheet.Pictures.Add(1, 9, "2.jpeg");
// Eklenen resim nesnesini al
Picture pic2 = worksheet.Pictures[imgIndex2];
//Resim 1'i resim 2'ye kopyalayın. Üst üste bindirilmiş iki resim 1 nesnesi elde edeceksiniz.
CopyOptions opt = new CopyOptions();
pic2.Copy(pic1, opt);
//Excel dosyasını kaydedin.
workbook.Save("result.xlsx");
```

### Ayrıca bakınız

* class [CopyOptions](../../../aspose.cells/copyoptions)
* class [Picture](../../picture)
* ad alanı [Aspose.Cells.Drawing](../../picture)
* toplantı [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
