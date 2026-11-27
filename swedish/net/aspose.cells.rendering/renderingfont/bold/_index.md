---
title: "RenderingFont.Bold"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RenderingFont-egenskap. Hämtar eller anger fetstil för teckensnittet"
type: docs
url: /sv/net/aspose.cells.rendering/renderingfont/bold/
---
## RenderingFont.Bold property

Hämtar eller sätter fetstil för typsnittet.

```csharp
public bool Bold { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Bold Font Example");

            // Skapa en stil för cellen
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            worksheet.Cells["A1"].SetStyle(style);

            // Skapa PDF-sparalternativ med vattenstämpel som demonstrerar fet teckensnitt
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Skapa renderingsfont med fet egenskap
            RenderingFont font = new RenderingFont("Arial", 36)
            {
                Bold = true,
                Color = System.Drawing.Color.Red
            };
            
            // Skapa vattenstämpel med fet teckensnitt
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font)
            {
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                Opacity = 0.3f
            };
            pdfSaveOptions.Watermark = watermark;

            // Spara arbetsboken
            workbook.Save("BoldFontExample.pdf", pdfSaveOptions);
        }
    }
}
```

### Se även

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


