---
title: "RenderingWatermark sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.RenderingWatermark sınıfı. İşleme için filigran."
type: docs
url: /tr/net/aspose.cells.rendering/renderingwatermark/
---
## RenderingWatermark class

Render için filigran.

```csharp
public class RenderingWatermark
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [RenderingWatermark](renderingwatermark/#constructor)(byte[]) | Görüntü filigranı örneği oluşturur. |
| [RenderingWatermark](renderingwatermark/#constructor_1)(string, RenderingFont) | Metin filigranı örneği oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Font](../../aspose.cells.rendering/renderingwatermark/font/) { get; } | Filigranın yazı tipini alır. |
| [HAlignment](../../aspose.cells.rendering/renderingwatermark/halignment/) { get; set; } | Filigranın sayfaya göre yatay hizalamasını alır veya ayarlar. |
| [Image](../../aspose.cells.rendering/renderingwatermark/image/) { get; } | Filigranın görüntüsünü alır. |
| [IsBackground](../../aspose.cells.rendering/renderingwatermark/isbackground/) { get; set; } | Filigranın sayfa içeriğinin arkasına yerleştirilip yerleştirilmeyeceğini gösterir. |
| [OffsetX](../../aspose.cells.rendering/renderingwatermark/offsetx/) { get; set; } | [`HAlignment`](./halignment/) için ofset değerini alır veya ayarlar. |
| [OffsetY](../../aspose.cells.rendering/renderingwatermark/offsety/) { get; set; } | [`VAlignment`](./valignment/) için ofset değerini alır veya ayarlar. |
| [Opacity](../../aspose.cells.rendering/renderingwatermark/opacity/) { get; set; } | Filigranın opaklığını [0, 1] aralığında alır veya ayarlar. |
| [Rotation](../../aspose.cells.rendering/renderingwatermark/rotation/) { get; set; } | Filigranın dönüş açısını derece cinsinden alır veya ayarlar. |
| [ScaleToPagePercent](../../aspose.cells.rendering/renderingwatermark/scaletopagepercent/) { get; set; } | Hedef sayfaya göre ölçeği yüzde olarak alır veya ayarlar. |
| [Text](../../aspose.cells.rendering/renderingwatermark/text/) { get; } | Filigranın metnini alır. |
| [VAlignment](../../aspose.cells.rendering/renderingwatermark/valignment/) { get; set; } | Filigranın sayfaya göre dikey hizalamasını alır veya ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing;

    public class RenderingWatermarkDemo
    {
        public static void RenderingWatermarkExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample worksheet.");

            // Filigran için bir yazı tipi oluştur
            RenderingFont font = new RenderingFont("Calibri", 68);
            font.Italic = true;
            font.Bold = true;
            font.Color = Color.Blue;

            // Metin ve belirtilen yazı tipinden bir filigran oluştur
            RenderingWatermark watermark = new RenderingWatermark("Watermark", font);

            // Filigran için özellikleri ayarla
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;
            watermark.Rotation = 30;
            watermark.Opacity = 0.6f;
            watermark.ScaleToPagePercent = 50;
            watermark.IsBackground = true;

            // PDF'ye işleme için filigranı belirt
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // Çalışma kitabını filigranlı bir PDF olarak kaydet
            workbook.Save("output_watermark.pdf", options);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


