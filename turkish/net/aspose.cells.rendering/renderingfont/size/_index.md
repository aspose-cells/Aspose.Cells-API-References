---
title: "RenderingFont.Size"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RenderingFont özelliği. Yazı tipinin nokta cinsinden boyutunu alır"
type: docs
url: /tr/net/aspose.cells.rendering/renderingfont/size/
---
## RenderingFont.Size property

Yazı tipinin boyutunu puan cinsinden alır.

```csharp
public float Size { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingFontPropertySizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // İlk yazı tipini oluşturun ve Size özelliğini okuma örneğini gösterin
            RenderingFont smallFont = new RenderingFont("Arial", 12);
            Console.WriteLine("Initial font size: " + smallFont.Size);

            // İlk yazı tipi boyutuyla filigran oluşturun
            PdfSaveOptions optionsSmall = new PdfSaveOptions
            {
                Watermark = new RenderingWatermark("CONFIDENTIAL", smallFont)
            };
            workbook.Save("SmallWatermark.pdf", optionsSmall);

            // Daha büyük boyutlu yeni bir yazı tipi oluşturun
            RenderingFont largeFont = new RenderingFont("Arial", 24);
            Console.WriteLine("Modified font size: " + largeFont.Size);

            // Daha büyük yazı tipi boyutuyla filigran oluşturun
            PdfSaveOptions optionsLarge = new PdfSaveOptions
            {
                Watermark = new RenderingWatermark("CONFIDENTIAL", largeFont)
            };
            workbook.Save("LargeWatermark.pdf", optionsLarge);
        }
    }
}
```

### Ayrıca Bakınız

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


