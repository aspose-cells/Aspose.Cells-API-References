---
title: "ImageOrPrintOptions.IsOptimized"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. Çıktı öğelerinin optimize edilip edilmediğini gösterir"
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/isoptimized/
---
## ImageOrPrintOptions.IsOptimized property

Çıktı öğelerinin optimize edilip edilmediğini gösterir.

```csharp
public bool IsOptimized { get; set; }
```

### Açıklamalar

Varsayılan değer false'tur. Şu anda bu özellik true olarak ayarlandığında, aşağıdaki iyileştirmeler yapılır: 1. kenar çizgilerini iyileştir. 2. Svg görüntüsüne render edilirken dosya boyutunu iyileştir.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyIsOptimizedDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i}-{j}");
                }
            }

            // Görüntü renderleme seçeneklerini ayarla
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // IsOptimized özelliğini göster
            options.IsOptimized = true; // Enable optimization
            
            // Sayfayı görüntüye render et
            SheetRender renderer = new SheetRender(sheet, options);
            MemoryStream stream = new MemoryStream();
            renderer.ToImage(0, stream);
            
            Console.WriteLine($"Image rendered with optimization: {options.IsOptimized}");
            Console.WriteLine($"Image size: {stream.Length} bytes");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


