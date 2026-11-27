---
title: "RenderingWatermark.Text"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RenderingWatermark-egenskap. Hämtar texten för vattenstämpeln"
type: docs
url: /sv/net/aspose.cells.rendering/renderingwatermark/text/
---
## RenderingWatermark.Text property

Hämtar texten för vattenstämpeln.

```csharp
public string Text { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingWatermarkPropertyTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa renderings­teckensnitt för vattenstämpeltext
            RenderingFont font = new RenderingFont("Arial", 36);

            // Initiera textvattenstämpel med teckensnittskonfiguration
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);

            // Visa aktuell vattenstämpeltext
            Console.WriteLine("Watermark Text: " + watermark.Text);

            // Konfigurera vattenstämpelns utseende
            watermark.Rotation = 45f;
            watermark.Opacity = 0.3f;
            watermark.IsBackground = true;
            watermark.ScaleToPagePercent = 150;

            // Applicera vattenstämpel på PDF‑sparalternativ
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark; // Fixed property name

            // Spara till PDF för att visualisera vattenstämpelseffekter
            workbook.Save("WatermarkDemo.pdf", options);
        }
    }
}
```

### Se även

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


