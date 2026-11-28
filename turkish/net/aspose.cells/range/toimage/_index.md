---
title: "Range.ToImage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Aralığı görüntüye dönüştürür"
type: docs
url: /tr/net/aspose.cells/range/toimage/
---
## Range.ToImage method

Aralığı görüntüye dönüştürür.

```csharp
public byte[] ToImage(ImageOrPrintOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| seçenekler | ImageOrPrintOptions | Bu aralığı görüntüye dönüştürme seçenekleri |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RangeMethodToImageWithImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Örnek Excel dosyasından bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook("example.xlsx");
            
            // İlk worksheet'i ve hücrelerini alın
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // A1:J25 aralığını oluşturun
            Aspose.Cells.Range range = cells.CreateRange("A1:J25");
            
            // Görüntü seçenekleri oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions()
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            
            // Aralığı görüntüye dönüştür
            byte[] imageData = range.ToImage(options);
            
            // Görüntüyü dosyaya kaydet
            File.WriteAllBytes("range_output.png", imageData);
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


