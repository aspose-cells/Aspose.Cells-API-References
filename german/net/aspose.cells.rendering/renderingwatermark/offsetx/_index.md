---
title: "RenderingWatermark.OffsetX"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RenderingWatermark-Eigenschaft. Gibt den Versatzwert für HAlignment zurück oder setzt ihn"
type: docs
url: /de/net/aspose.cells.rendering/renderingwatermark/offsetx/
---
## RenderingWatermark.OffsetX property

Gibt den Versatzwert für [`HAlignment`](../halignment/) zurück oder setzt ihn

```csharp
public float OffsetX { get; set; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyOffsetXDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Sample Data");

            RenderingFont font = new RenderingFont("Arial", 24)
            {
                Color = Color.Red,
                Bold = true
            };

            RenderingWatermark watermark = new RenderingWatermark("DEMO WATERMARK", font)
            {
                Rotation = 45,
                Opacity = 0.3f,
                IsBackground = true,
                OffsetX = 100,  // Demonstrating OffsetX property
                OffsetY = 50
            };

            PdfSaveOptions options = new PdfSaveOptions
            {
                Watermark = watermark
            };

            workbook.Save("WatermarkWithOffsetX.pdf", options);
        }
    }
}
```

### Siehe auch

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


