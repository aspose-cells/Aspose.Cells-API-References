---
title: "RenderingWatermark.HAlignment"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RenderingWatermark özelliği. Filigranın sayfaya yatay hizalamasını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.rendering/renderingwatermark/halignment/
---
## RenderingWatermark.HAlignment property

Filigranın sayfaya göre yatay hizalamasını alır veya ayarlar.

```csharp
public TextAlignmentType HAlignment { get; set; }
```

### Açıklamalar

Yalnızca Sol, Orta, Sağ geçerlidir. Varsayılan Sol'tur.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyHAlignmentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Watermark HAlignment Demo");

            // PDF kaydetme seçeneklerini oluşturun
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Farklı HAlignment ayarlarıyla filigran oluştur ve yapılandır
            RenderingFont font = new RenderingFont("Arial", 48)
            {
                Bold = true,
                Color = System.Drawing.Color.Blue
            };

            // Orta hizalama ile filigran oluştur
            RenderingWatermark watermark = new RenderingWatermark("CENTER ALIGNED", font)
            {
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                Opacity = 0.5f
            };
            pdfSaveOptions.Watermark = watermark;

            // Orta hizalı filigranla kaydet
            workbook.Save("WatermarkCenterAlignment.pdf", pdfSaveOptions);

            // Sol hizalamaya değiştir
            watermark.HAlignment = TextAlignmentType.Left;
            workbook.Save("WatermarkLeftAlignment.pdf", pdfSaveOptions);

            // Sağ hizalamaya değiştir
            watermark.HAlignment = TextAlignmentType.Right;
            workbook.Save("WatermarkRightAlignment.pdf", pdfSaveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


