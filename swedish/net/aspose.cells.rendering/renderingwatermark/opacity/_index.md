---
title: "RenderingWatermark.Opacity"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RenderingWatermark-egenskap. Hämtar eller anger opaciteten för vattenstämpeln i intervallet 0‑1"
type: docs
url: /sv/net/aspose.cells.rendering/renderingwatermark/opacity/
---
## RenderingWatermark.Opacity property

Hämtar eller anger opaciteten för vattenstämpeln i intervallet [0, 1].

```csharp
public float Opacity { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyOpacityDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample content");

            RenderingFont font = new RenderingFont("Arial", 72);
            font.Bold = true;
            font.Color = Color.Blue;

            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
            watermark.Opacity = 0.4f;
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;
            watermark.IsBackground = true;

            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            workbook.Save("WatermarkOpacityDemo.pdf", options);
        }
    }
}
```

### Se även

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


