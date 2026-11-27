---
title: "RenderingWatermark.IsBackground"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RenderingWatermark-egenskap. Anger om vattenstämpeln placeras bakom sidans innehåll"
type: docs
url: /sv/net/aspose.cells.rendering/renderingwatermark/isbackground/
---
## RenderingWatermark.IsBackground property

Anger om vattenstämpeln placeras bakom sidans innehåll.

```csharp
public bool IsBackground { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Sample Content");

            // Skapa vattenstämpel med IsBackground satt till true
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

            // Konfigurera sparaalternativ med vattenstämpel
            PdfSaveOptions options = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // Spara med bakgrundsvattenstämpel
            workbook.Save("WatermarkIsBackgroundDemo.pdf", options);
        }
    }
}
```

### Se även

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


