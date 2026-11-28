---
title: "ImageOrPrintOptions.Quality"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. Oluşturulan görüntülerin kalitesini belirleyen bir değeri alır veya ayarlar; bu değer yalnızca sayfalar JPEG formatında kaydedilirken uygulanır. Varsayılan değer 100'tür"
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/quality/
---
## ImageOrPrintOptions.Quality property

Sayfaları `Jpeg` formatında kaydederken uygulanacak, oluşturulan görüntülerin kalitesini belirleyen bir değeri alır veya ayarlar. Varsayılan değer 100.

```csharp
public int Quality { get; set; }
```

### Açıklamalar

Yalnızca JPEG olarak kaydederken etkili olur. Değer 0 ile 100 arasında olmalıdır. Varsayılan değer 100'tür.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyQualityDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["C3"].PutValue(DateTime.Now);

            // Farklı kalite ayarlarıyla görüntü seçenekleri oluşturun
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;
            options.Quality = 100; // Highest quality

            // Çalışma sayfasını yüksek kaliteyle görüntüye dönüştür
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "HighQualityOutput.jpg");

            // Farkı göstermek için kaliteyi değiştirin
            options.Quality = 50; // Medium quality
            renderer.ToImage(0, "MediumQualityOutput.jpg");

            options.Quality = 10; // Low quality
            renderer.ToImage(0, "LowQualityOutput.jpg");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


