---
title: "Picture.PlaceInCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Picture yöntemi. Bu resmi hücreye yerleştir"
type: docs
url: /tr/net/aspose.cells.drawing/picture/placeincell/
---
## Picture.PlaceInCell method

Bu resmi hücreye yerleştir

```csharp
[Obsolete("Use Picture.IsPlacedInCell property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void PlaceInCell()
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine, lütfen Picture.IsPlacedInCell özelliğini kullanın. Bu özellik Ocak 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureMethodPlaceInCellDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir resim ekle
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Resmi A1 hücresine yerleştir
            picture.PlaceInCell();

            // Resmin hücreye yerleştirildiğini doğrula
            Cell cell = worksheet.Cells["A1"];
            byte[] imageData = cell.EmbeddedImage;
            Console.WriteLine("Image placed in cell A1. Image data length: " + imageData.Length);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


