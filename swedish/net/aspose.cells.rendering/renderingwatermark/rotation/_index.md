---
title: "RenderingWatermark.Rotation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RenderingWatermark-egenskap. Hämtar eller anger rotation av vattenstämpeln i grader"
type: docs
url: /sv/net/aspose.cells.rendering/renderingwatermark/rotation/
---
## RenderingWatermark.Rotation property

Hämtar eller anger rotation av vattenstämpeln i grader.

```csharp
public float Rotation { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyRotationDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data for watermark demo");

            // Skapa teckensnitt för vattenstämpel
            RenderingFont font = new RenderingFont("Arial", 72);
            font.Color = Color.FromArgb(128, 0, 0, 255);
            font.Bold = true;

            // Skapa vattenstämpel med rotation
            RenderingWatermark watermark = new RenderingWatermark("ROTATED WATERMARK", font);
            watermark.Rotation = 45; // 45 degree rotation
            watermark.Opacity = 0.5f;
            watermark.IsBackground = true;

            // Ställ in PDF‑sparalternativ med vattenstämpel
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // Spara med vattenstämpel
            workbook.Save("WatermarkRotationDemo.pdf", options);
        }
    }
}
```

### Se även

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


