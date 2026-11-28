---
title: "ShapeCollection.AddLinkedPicture"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Bağlantılı bir resim ekle"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addlinkedpicture/
---
## ShapeCollection.AddLinkedPicture method

Bağlantılı bir resim ekle.

```csharp
public Picture AddLinkedPicture(int topRow, int leftColumn, int height, int width, 
    string sourceFullName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| yükseklik | Int32 | Şeklin yüksekliği. Piksel biriminde |
| genişlik | Int32 | Şeklin genişliği. Piksel biriminde |
| sourceFullName | String | Bağlantılı görüntünün kaynak dosyasının yolu ve adı |

### Dönüş Değeri

[`Picture`](../../picture/) Picture object.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLinkedPictureWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresine örnek metin ekle
            worksheet.Cells["A1"].PutValue("Image will be linked below:");
            
            // Çalışma sayfasına bağlantılı resim ekle
            string imageUrl = "https://example.com/sample.jpg";
            worksheet.Shapes.AddLinkedPicture(1, 1, 100, 100, imageUrl);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output_with_linked_picture.xlsx");
            
            Console.WriteLine("Workbook saved with linked picture.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


