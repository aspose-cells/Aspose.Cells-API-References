---
title: "PictureCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PictureCollection özelliği. Belirtilen indeksteki Picture öğesini alır"
type: docs
url: /tr/net/aspose.cells.drawing/picturecollection/item/
---
## PictureCollection indexer

Belirtilen indeksteki [`Picture`](../../picture/) öğesini alır.

```csharp
public Picture this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Öğenin sıfır tabanlı indeksi. |

### Dönüş Değeri

Belirtilen indeksteki öğe.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Resim koleksiyonunu al
            PictureCollection pictures = worksheet.Pictures;
            
            // Bir resim ekle ("image.png" yerine gerçek resim yolunu koyun)
            int index = pictures.Add(1, 1, "image.png");
            
            // Item özelliğini kullanarak resme erişin
            Picture pic = pictures[index];
            
            // Item özelliğinin kullanımını göster
            Console.WriteLine($"Picture at index {index} has width: {pic.Width} and height: {pic.Height}");
            
            // Resim özelliklerini değiştir
            pic.Height = 200;
            pic.Width = 300;
            
            // Çalışma kitabını kaydedin
            workbook.Save("PictureCollectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Picture](../../picture/)
* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


