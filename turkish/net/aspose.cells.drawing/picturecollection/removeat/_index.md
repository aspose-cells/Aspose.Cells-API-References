---
title: "PictureCollection.RemoveAt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PictureCollection yöntemi. Belirli indeksteki şekilleri kaldırır"
type: docs
url: /tr/net/aspose.cells.drawing/picturecollection/removeat/
---
## PictureCollection.RemoveAt method

Belirli indeksteki şekilleri kaldır.

```csharp
public void RemoveAt(int index)
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı resimler ekle
            int index1 = worksheet.Pictures.Add(1, 1, "image1.png");
            int index2 = worksheet.Pictures.Add(5, 1, "image2.png");
            int index3 = worksheet.Pictures.Add(10, 1, "image3.png");

            Console.WriteLine("Number of pictures before removal: " + worksheet.Pictures.Count);

            // Belirtilen indeksteki resmi kaldır
            worksheet.Pictures.RemoveAt(index2);

            Console.WriteLine("Number of pictures after removal: " + worksheet.Pictures.Count);
        }
    }
}
```

### Ayrıca Bakınız

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


