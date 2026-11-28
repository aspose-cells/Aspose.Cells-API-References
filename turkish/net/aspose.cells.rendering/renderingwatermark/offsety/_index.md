---
title: "RenderingWatermark.OffsetY"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RenderingWatermark özelliği. Ofset değerini VAlignment'a alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.rendering/renderingwatermark/offsety/
---
## RenderingWatermark.OffsetY property

[`VAlignment`](../valignment/) için ofset değerini alır veya ayarlar

```csharp
public float OffsetY { get; set; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyOffsetYDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("OffsetY Demo");

            // Filigran yazı tipini oluştur
            RenderingFont font = new RenderingFont("Arial", 24)
            {
                Color = Color.Red,
                Bold = true
            };

            // Farklı OffsetY değerleriyle filigran oluştur
            RenderingWatermark watermark = new RenderingWatermark("VERTICAL OFFSET", font)
            {
                Rotation = 0,
                Opacity = 0.3f,
                IsBackground = true,
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                OffsetX = 0,
                OffsetY = 100 // Demonstrating OffsetY property
            };

            // Filigranlı kaydetme seçeneklerini ayarla
            PdfSaveOptions options = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // Filigran ofsetiyle kaydet
            workbook.Save("WatermarkOffsetYDemo.pdf", options);
        }
    }
}
```

### Ayrıca Bakınız

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


