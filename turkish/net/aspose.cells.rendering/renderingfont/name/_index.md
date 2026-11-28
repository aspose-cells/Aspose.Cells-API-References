---
title: "RenderingFont.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RenderingFont özelliği. Yazı tipinin adını alır"
type: docs
url: /tr/net/aspose.cells.rendering/renderingfont/name/
---
## RenderingFont.Name property

Yazı tipinin adını alır.

```csharp
public string Name { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingFontPropertyNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // PDF kaydetme seçeneklerini oluşturun
            PdfSaveOptions options = new PdfSaveOptions();

            // İlk rendering yazı tipini "Arial" ile oluşturun
            RenderingFont fontArial = new RenderingFont("Arial", 16);
            Console.WriteLine("Initial font name: " + fontArial.Name);

            // İlk yazı tipiyle filigran oluşturun
            RenderingWatermark watermark = new RenderingWatermark("Confidential", fontArial);
            watermark.Opacity = 0.5f;
            watermark.Rotation = 45;
            options.Watermark = watermark;

            // İlk yazı tipi filigranı ile kaydedin
            workbook.Save("WatermarkInitial.pdf", options);

            // Yeni rendering yazı tipini "Times New Roman" ile oluşturun
            RenderingFont fontTimesNewRoman = new RenderingFont("Times New Roman", 16);
            Console.WriteLine("\nModified font name: " + fontTimesNewRoman.Name);

            // Yeni yazı tipiyle filigranı güncelleyin
            RenderingWatermark updatedWatermark = new RenderingWatermark("Confidential", fontTimesNewRoman);
            updatedWatermark.Opacity = 0.5f;
            updatedWatermark.Rotation = 45;
            options.Watermark = updatedWatermark;

            // Değiştirilmiş yazı tipi filigranı ile kaydedin
            workbook.Save("WatermarkModified.pdf", options);
        }
    }
}
```

### Ayrıca Bakınız

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


