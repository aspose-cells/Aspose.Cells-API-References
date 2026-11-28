---
title: "RenderingWatermark.Font"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RenderingWatermark özelliği. Filigranın yazı tipini alır"
type: docs
url: /tr/net/aspose.cells.rendering/renderingwatermark/font/
---
## RenderingWatermark.Font property

Filigranın yazı tipini alır.

```csharp
public RenderingFont Font { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingWatermarkPropertyFontDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir renderleme yazı tipi oluştur ve başlangıç özelliklerini ayarla
            RenderingFont font = new RenderingFont("Arial", 24);
            
            // Renderleme yazı tipiyle bir metin filigranı oluştur
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
            
            // İlk yazı tipi özelliklerini göster
            Console.WriteLine("Initial Font Name: " + watermark.Font.Name);
            Console.WriteLine("Initial Font Size: " + watermark.Font.Size);
            Console.WriteLine("Initial Bold Status: " + watermark.Font.Bold);
            
            // RenderingFont referansı aracılığıyla yazı tipi özelliklerini değiştir
            font.Bold = true;
            
            // Filigrandan güncellenmiş yazı tipi özelliklerini göster
            Console.WriteLine("\nUpdated Font Name: " + watermark.Font.Name);
            Console.WriteLine("Updated Font Size: " + watermark.Font.Size);
            Console.WriteLine("Updated Bold Status: " + watermark.Font.Bold);
            
            // Filigran görüntüleme özelliklerini yapılandır
            watermark.Opacity = 0.5f;
            watermark.Rotation = 45;
            watermark.IsBackground = true;
            
            // PDF kaydetme seçeneklerini oluştur ve filigranı ata
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.Watermark = watermark;
            
            // Yazı tipi değişikliklerini göstermek için filigranlı PDF ile çalışma kitabını kaydet
            workbook.Save("RenderingWatermarkFontDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [RenderingFont](../../renderingfont/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


