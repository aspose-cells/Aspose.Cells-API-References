---
title: "PdfSaveOptions.Watermark"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSaveOptions-egenskap. Hämtar eller anger vattenstämpel för utdata"
type: docs
url: /sv/net/aspose.cells/pdfsaveoptions/watermark/
---
## PdfSaveOptions.Watermark property

Hämtar eller anger vattenstämpel för utdata.

```csharp
public RenderingWatermark Watermark { get; set; }
```

### Exempel

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
            // Skapa en arbetsbok med 3 kalkylblad
            Workbook wb = new Workbook();
            wb.Worksheets[0].Cells["A1"].PutValue("Page1");
            int index = wb.Worksheets.Add();
            wb.Worksheets[index].Cells["A1"].PutValue("Page2");
            index = wb.Worksheets.Add();
            wb.Worksheets[index].Cells["A1"].PutValue("Page3");

            // Skapa teckensnitt för vattenstämpel
            RenderingFont font = new RenderingFont("Calibri", 68);
            font.Italic = true;
            font.Bold = true;
            font.Color = Color.Blue;

            // Skapa vattenstämpel med text och teckensnitt
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;
            watermark.Rotation = 45;
            watermark.Opacity = 0.3f;
            watermark.ScaleToPagePercent = 75;

            // Ange vattenstämpel i PDF-sparalternativ
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // Spara arbetsbok med vattenstämpel
            wb.Save("output_watermark.pdf", options);
        }
    }
}
```

### Se även

* class [RenderingWatermark](../../../aspose.cells.rendering/renderingwatermark/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


