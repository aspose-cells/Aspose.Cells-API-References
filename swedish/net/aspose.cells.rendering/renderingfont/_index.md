---
title: "Klass RenderingFont"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.RenderingFont‑klass. Typsnitt för rendering"
type: docs
url: /sv/net/aspose.cells.rendering/renderingfont/
---
## RenderingFont class

Typsnitt för rendering.

```csharp
public class RenderingFont
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [RenderingFont](renderingfont/)(string, float) | Initierar en ny instans av `RenderingFont` |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Bold](../../aspose.cells.rendering/renderingfont/bold/) { get; set; } | Hämtar eller sätter fetstil för typsnittet. |
| [Color](../../aspose.cells.rendering/renderingfont/color/) { get; set; } | Hämtar eller sätter färg för typsnittet. |
| [Italic](../../aspose.cells.rendering/renderingfont/italic/) { get; set; } | Hämtar eller sätter kursiv för typsnittet. |
| [Name](../../aspose.cells.rendering/renderingfont/name/) { get; } | Hämtar namn på typsnittet. |
| [Size](../../aspose.cells.rendering/renderingfont/size/) { get; } | Hämtar storlek på typsnittet i punkter. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            sheet.Cells["A1"].PutValue("Hello World!");

            // Skapa ett RenderingFont‑objekt
            RenderingFont renderingFont = new RenderingFont("Arial", 12)
            {
                Bold = true,
                Italic = true,
                Color = Color.Blue
            };

            // Skapa ett RenderingWatermark-objekt med RenderingFont
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

            // Skapa PdfSaveOptions och ställ in vattenstämpeln
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions
            {
                Watermark = watermark,
                EmbedStandardWindowsFonts = true,
                CalculateFormula = true,
                ExportDocumentStructure = true,
                DisplayDocTitle = true
            };

            // Spara arbetsboken som PDF med vattenstämpeln
            workbook.Save("RenderingFontExample.pdf", pdfSaveOptions);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


