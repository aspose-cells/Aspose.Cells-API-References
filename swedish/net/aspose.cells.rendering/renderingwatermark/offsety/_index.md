---
title: "RenderingWatermark.OffsetY"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RenderingWatermark-egenskap. Hämtar eller anger förskjutningsvärde till VAlignment"
type: docs
url: /sv/net/aspose.cells.rendering/renderingwatermark/offsety/
---
## RenderingWatermark.OffsetY property

Hämtar eller anger förskjutningsvärde till [`VAlignment`](../valignment/)

```csharp
public float OffsetY { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("OffsetY Demo");

            // Skapa teckensnitt för vattenstämpel
            RenderingFont font = new RenderingFont("Arial", 24)
            {
                Color = Color.Red,
                Bold = true
            };

            // Skapa vattenstämpel med olika OffsetY-värden
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

            // Ställ in sparalternativ med vattenstämpel
            PdfSaveOptions options = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // Spara med vattenstämpelns förskjutning
            workbook.Save("WatermarkOffsetYDemo.pdf", options);
        }
    }
}
```

### Se även

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


