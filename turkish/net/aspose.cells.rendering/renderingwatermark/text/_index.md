---
title: "RenderingWatermark.Text"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RenderingWatermark özelliği. Filigranın metnini alır"
type: docs
url: /tr/net/aspose.cells.rendering/renderingwatermark/text/
---
## RenderingWatermark.Text property

Filigranın metnini alır.

```csharp
public string Text { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingWatermarkPropertyTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Filigran metni için işleme yazı tipini oluştur
            RenderingFont font = new RenderingFont("Arial", 36);

            // Yazı tipi yapılandırmasıyla metin filigranını başlat
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);

            // Mevcut filigran metnini göster
            Console.WriteLine("Watermark Text: " + watermark.Text);

            // Filigran görünümünü yapılandır
            watermark.Rotation = 45f;
            watermark.Opacity = 0.3f;
            watermark.IsBackground = true;
            watermark.ScaleToPagePercent = 150;

            // Filigranı PDF kaydetme seçeneklerine uygula
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark; // Fixed property name

            // Filigran etkilerini görselleştirmek için PDF olarak kaydet
            workbook.Save("WatermarkDemo.pdf", options);
        }
    }
}
```

### Ayrıca Bakınız

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


