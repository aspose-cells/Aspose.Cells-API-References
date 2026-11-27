---
title: "Klass RenderingWatermark"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.RenderingWatermark-klass. Vattenstämpel för rendering"
type: docs
url: /sv/net/aspose.cells.rendering/renderingwatermark/
---
## RenderingWatermark class

Vattenstämpel för rendering.

```csharp
public class RenderingWatermark
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [RenderingWatermark](renderingwatermark/#constructor)(byte[]) | Skapar en instans av bildvattenstämpel. |
| [RenderingWatermark](renderingwatermark/#constructor_1)(string, RenderingFont) | Skapar en instans av textvattenstämpel. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Font](../../aspose.cells.rendering/renderingwatermark/font/) { get; } | Hämtar teckensnittet för vattenstämpeln. |
| [HAlignment](../../aspose.cells.rendering/renderingwatermark/halignment/) { get; set; } | Hämtar eller anger horisontell justering av vattenstämpeln på sidan. |
| [Image](../../aspose.cells.rendering/renderingwatermark/image/) { get; } | Hämtar bilden av vattenstämpeln. |
| [IsBackground](../../aspose.cells.rendering/renderingwatermark/isbackground/) { get; set; } | Anger om vattenstämpeln placeras bakom sidans innehåll. |
| [OffsetX](../../aspose.cells.rendering/renderingwatermark/offsetx/) { get; set; } | Hämtar eller anger förskjutningsvärde till [`HAlignment`](./halignment/) |
| [OffsetY](../../aspose.cells.rendering/renderingwatermark/offsety/) { get; set; } | Hämtar eller anger förskjutningsvärde till [`VAlignment`](./valignment/) |
| [Opacity](../../aspose.cells.rendering/renderingwatermark/opacity/) { get; set; } | Hämtar eller anger opaciteten för vattenstämpeln i intervallet [0, 1]. |
| [Rotation](../../aspose.cells.rendering/renderingwatermark/rotation/) { get; set; } | Hämtar eller anger rotation av vattenstämpeln i grader. |
| [ScaleToPagePercent](../../aspose.cells.rendering/renderingwatermark/scaletopagepercent/) { get; set; } | Hämtar eller anger skala relativt målsidan i procent. |
| [Text](../../aspose.cells.rendering/renderingwatermark/text/) { get; } | Hämtar texten för vattenstämpeln. |
| [VAlignment](../../aspose.cells.rendering/renderingwatermark/valignment/) { get; set; } | Hämtar eller anger vertikal justering av vattenstämpeln på sidan. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample worksheet.");

            // Skapa ett teckensnitt för vattenstämpeln
            RenderingFont font = new RenderingFont("Calibri", 68);
            font.Italic = true;
            font.Bold = true;
            font.Color = Color.Blue;

            // Skapa en vattenstämpel från text och det angivna teckensnittet
            RenderingWatermark watermark = new RenderingWatermark("Watermark", font);

            // Ange egenskaper för vattenstämpeln
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;
            watermark.Rotation = 30;
            watermark.Opacity = 0.6f;
            watermark.ScaleToPagePercent = 50;
            watermark.IsBackground = true;

            // Specificera vattenstämpel för rendering till PDF
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // Spara arbetsboken som PDF med vattenstämpeln
            workbook.Save("output_watermark.pdf", options);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


