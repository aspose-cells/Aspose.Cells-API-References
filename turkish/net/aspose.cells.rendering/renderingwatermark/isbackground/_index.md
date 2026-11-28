---
title: "RenderingWatermark.IsBackground"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RenderingWatermark özelliği. Filigranın sayfa içeriğinin arkasına yerleştirilip yerleştirilmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells.rendering/renderingwatermark/isbackground/
---
## RenderingWatermark.IsBackground property

Filigranın sayfa içeriğinin arkasına yerleştirilip yerleştirilmeyeceğini gösterir.

```csharp
public bool IsBackground { get; set; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyIsBackgroundDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("Sample Content");

            // IsBackground true olarak ayarlanmış filigran oluştur
            RenderingFont font = new RenderingFont("Arial", 36)
            {
                Color = Color.LightGray
            };
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font)
            {
                IsBackground = true,
                Rotation = 45,
                Opacity = 0.2f
            };

            // Filigran ile kaydetme seçeneklerini yapılandır
            PdfSaveOptions options = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // Arka plan filigranı ile kaydet
            workbook.Save("WatermarkIsBackgroundDemo.pdf", options);
        }
    }
}
```

### Ayrıca Bakınız

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


