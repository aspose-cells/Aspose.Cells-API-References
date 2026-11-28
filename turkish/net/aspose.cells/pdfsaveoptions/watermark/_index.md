---
title: "PdfSaveOptions.Watermark"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSaveOptions özelliği. Çıktıya uygulanacak filigranı alır veya ayarlar."
type: docs
url: /tr/net/aspose.cells/pdfsaveoptions/watermark/
---
## PdfSaveOptions.Watermark property

Çıktıya filigranı alır veya ayarlar.

```csharp
public RenderingWatermark Watermark { get; set; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyWatermarkDemo
    {
        public static void Run()
        {
            // 3 çalışma sayfası içeren bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            wb.Worksheets[0].Cells["A1"].PutValue("Page1");
            int index = wb.Worksheets.Add();
            wb.Worksheets[index].Cells["A1"].PutValue("Page2");
            index = wb.Worksheets.Add();
            wb.Worksheets[index].Cells["A1"].PutValue("Page3");

            // Filigran yazı tipini oluştur
            RenderingFont font = new RenderingFont("Calibri", 68);
            font.Italic = true;
            font.Bold = true;
            font.Color = Color.Blue;

            // Metin ve yazı tipi ile filigran oluştur
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;
            watermark.Rotation = 45;
            watermark.Opacity = 0.3f;
            watermark.ScaleToPagePercent = 75;

            // PDF kaydetme seçeneklerinde filigranı ayarla
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // Filigranlı çalışma kitabını kaydet
            wb.Save("output_watermark.pdf", options);
        }
    }
}
```

### Ayrıca Bakınız

* class [RenderingWatermark](../../../aspose.cells.rendering/renderingwatermark/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


