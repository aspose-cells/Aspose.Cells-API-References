---
title: "Class RenderingFont"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.RenderingFont sınıfı. Renderleme için yazı tipi"
type: docs
url: /tr/net/aspose.cells.rendering/renderingfont/
---
## RenderingFont class

Render için yazı tipi.

```csharp
public class RenderingFont
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [RenderingFont](renderingfont/)(string, float) | Yeni bir `RenderingFont` örneği başlatır |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Bold](../../aspose.cells.rendering/renderingfont/bold/) { get; set; } | Yazı tipinin kalınlığını alır veya ayarlar. |
| [Color](../../aspose.cells.rendering/renderingfont/color/) { get; set; } | Yazı tipinin rengini alır veya ayarlar. |
| [Italic](../../aspose.cells.rendering/renderingfont/italic/) { get; set; } | Yazı tipinin italik özelliğini alır veya ayarlar. |
| [Name](../../aspose.cells.rendering/renderingfont/name/) { get; } | Yazı tipinin adını alır. |
| [Size](../../aspose.cells.rendering/renderingfont/size/) { get; } | Yazı tipinin boyutunu puan cinsinden alır. |

### Örnekler

```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontDemo
    {
        public static void RenderingFontExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            sheet.Cells["A1"].PutValue("Hello World!");

            // Bir RenderingFont nesnesi oluştur
            RenderingFont renderingFont = new RenderingFont("Arial", 12)
            {
                Bold = true,
                Italic = true,
                Color = Color.Blue
            };

            // RenderingFont kullanarak bir RenderingWatermark nesnesi oluştur
            RenderingWatermark watermark = new RenderingWatermark("Sample Watermark", renderingFont)
            {
                Rotation = 45,
                ScaleToPagePercent = 100,
                Opacity = 0.5f,
                IsBackground = true,
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                OffsetX = 0,
                OffsetY = 0
            };

            // PdfSaveOptions oluştur ve filigranı ayarla
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions
            {
                Watermark = watermark,
                EmbedStandardWindowsFonts = true,
                CalculateFormula = true,
                ExportDocumentStructure = true,
                DisplayDocTitle = true
            };

            // Çalışma kitabını filigranlı PDF olarak kaydet
            workbook.Save("RenderingFontExample.pdf", pdfSaveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


