---
title: "RenderingWatermark.VAlignment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RenderingWatermark-egenskap. Hämtar eller anger vertikal justering av vattenstämpeln till sidan"
type: docs
url: /sv/net/aspose.cells.rendering/renderingwatermark/valignment/
---
## RenderingWatermark.VAlignment property

Hämtar eller anger vertikal justering av vattenstämpeln på sidan.

```csharp
public TextAlignmentType VAlignment { get; set; }
```

### Anmärkningar

Endast Top, Center, Bottom är giltiga. Standard är Top.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyVAlignmentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Watermark VAlignment Demo");

            // Skapa PDF-sparalternativ
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Skapa och konfigurera vattenstämpel med olika VAlignment-inställningar
            RenderingFont font = new RenderingFont("Arial", 48)
            {
                Bold = true,
                Color = System.Drawing.Color.Red
            };

            // Skapa vattenstämpel med vertikal justering satt till Center
            RenderingWatermark watermark = new RenderingWatermark("CENTER ALIGNED", font)
            {
                VAlignment = TextAlignmentType.Center,
                HAlignment = TextAlignmentType.Center,
                Opacity = 0.5f
            };
            pdfSaveOptions.Watermark = watermark;

            // Spara arbetsboken med vattenstämpel
            workbook.Save("WatermarkVAlignmentDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Se även

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


