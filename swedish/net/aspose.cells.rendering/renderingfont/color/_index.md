---
title: "RenderingFont.Color"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RenderingFont-egenskap. Hämtar eller anger färg för teckensnittet"
type: docs
url: /sv/net/aspose.cells.rendering/renderingfont/color/
---
## RenderingFont.Color property

Hämtar eller sätter färg för typsnittet.

```csharp
public Color Color { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Testing font color property");

            RenderingFont font = new RenderingFont("Arial", 16);
            font.Color = System.Drawing.Color.Red;
            font.Bold = true;

            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = new RenderingWatermark("COLOR DEMO", font)
            {
                Opacity = 0.5f,
                IsBackground = true
            };

            workbook.Save("FontColorDemo.pdf", options);
        }
    }
}
```

### Se även

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


