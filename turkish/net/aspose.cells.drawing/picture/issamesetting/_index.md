---
title: IsSameSetting
second_title: Aspose.Cells for .NET API Referansı
description: Şeklin aynı olup olmadığını döndürür.
type: docs
weight: 190
url: /tr/net/aspose.cells.drawing/picture/issamesetting/
---
## Picture.IsSameSetting method

Şeklin aynı olup olmadığını döndürür.

```csharp
public override bool IsSameSetting(object obj)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| obj | Object |  |

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
if(pic1.IsSameSetting(pic1))
{
    //iki görüntü nesnesi aynıdır.
}

if(!pic1.IsSameSetting(pic2))
{
    // iki görüntü nesnesi aynı değil.
}
```

### Ayrıca bakınız

* class [Picture](../../picture)
* ad alanı [Aspose.Cells.Drawing](../../picture)
* toplantı [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
