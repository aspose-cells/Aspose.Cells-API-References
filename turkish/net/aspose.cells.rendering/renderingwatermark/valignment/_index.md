---
title: "RenderingWatermark.VAlignment"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RenderingWatermark özelliği. Filigranın sayfaya dikey hizalamasını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.rendering/renderingwatermark/valignment/
---
## RenderingWatermark.VAlignment property

Filigranın sayfaya göre dikey hizalamasını alır veya ayarlar.

```csharp
public TextAlignmentType VAlignment { get; set; }
```

### Açıklamalar

Yalnızca Top, Center, Bottom geçerlidir. Varsayılan Top'tur.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyVAlignmentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Watermark VAlignment Demo");

            // PDF kaydetme seçeneklerini oluşturun
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Farklı VAlignment ayarlarıyla filigran oluştur ve yapılandır
            RenderingFont font = new RenderingFont("Arial", 48)
            {
                Bold = true,
                Color = System.Drawing.Color.Red
            };

            // Dikey hizalama Center olarak ayarlanmış filigran oluştur
            RenderingWatermark watermark = new RenderingWatermark("CENTER ALIGNED", font)
            {
                VAlignment = TextAlignmentType.Center,
                HAlignment = TextAlignmentType.Center,
                Opacity = 0.5f
            };
            pdfSaveOptions.Watermark = watermark;

            // Çalışma kitabını filigran ile kaydet
            workbook.Save("WatermarkVAlignmentDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


