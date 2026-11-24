---
title: "RenderingFont.Color"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RenderingFont-Eigenschaft. Gibt die Farbe der Schriftart zurück oder legt sie fest."
type: docs
url: /de/net/aspose.cells.rendering/renderingfont/color/
---
## RenderingFont.Color property

Liest oder setzt die Farbe für die Schriftart.

```csharp
public Color Color { get; set; }
```

### Beispiele

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

### Siehe auch

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


