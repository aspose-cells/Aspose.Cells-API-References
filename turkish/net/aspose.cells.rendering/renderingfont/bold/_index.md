---
title: "RenderingFont.Bold"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RenderingFont özelliği. Yazı tipi için kalınlığı alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.rendering/renderingfont/bold/
---
## RenderingFont.Bold property

Yazı tipinin kalınlığını alır veya ayarlar.

```csharp
public bool Bold { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontPropertyBoldDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Bold Font Example");

            // Hücre için bir stil oluştur
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            worksheet.Cells["A1"].SetStyle(style);

            // Kalın yazı tipini gösteren filigran ile PDF kaydetme seçenekleri oluştur
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Kalın özelliği olan renderleme yazı tipini oluştur
            RenderingFont font = new RenderingFont("Arial", 36)
            {
                Bold = true,
                Color = System.Drawing.Color.Red
            };
            
            // Kalın yazı tipli bir filigran oluştur
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font)
            {
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                Opacity = 0.3f
            };
            pdfSaveOptions.Watermark = watermark;

            // Çalışma kitabını kaydedin
            workbook.Save("BoldFontExample.pdf", pdfSaveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


