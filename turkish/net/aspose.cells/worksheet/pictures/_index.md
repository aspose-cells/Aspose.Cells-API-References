---
title: "Worksheet.Pictures"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Bir Picture koleksiyonu alır"
type: docs
url: /tr/net/aspose.cells/worksheet/pictures/
---
## Worksheet.Pictures property

Bir [`Picture`](../../../aspose.cells.drawing/picture/) koleksiyonu alır.

```csharp
public PictureCollection Pictures { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPicturesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir resim ekle
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Resim özelliklerini ayarla
            picture.Placement = PlacementType.FreeFloating;
            picture.BorderLineColor = System.Drawing.Color.Blue;
            picture.BorderWeight = 1;

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Kaydedilmiş çalışma kitabını doğrulamak için yükle
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Number of pictures: " + loadedWorkbook.Worksheets[0].Pictures.Count);
        }
    }
}
```

### Ayrıca Bakınız

* class [PictureCollection](../../../aspose.cells.drawing/picturecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


