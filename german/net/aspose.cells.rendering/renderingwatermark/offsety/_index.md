---
title: "RenderingWatermark.OffsetY"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RenderingWatermark property. Gibt den Versatzwert für VAlignment zurück oder setzt ihn"
type: docs
url: /de/net/aspose.cells.rendering/renderingwatermark/offsety/
---
## RenderingWatermark.OffsetY property

Gibt den Versatzwert für [`VAlignment`](../valignment/) zurück oder setzt ihn

```csharp
public float OffsetY { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("OffsetY Demo");

            // Erstellen Sie die Wasserzeichen-Schriftart
            RenderingFont font = new RenderingFont("Arial", 24)
            {
                Color = Color.Red,
                Bold = true
            };

            // Wasserzeichen mit unterschiedlichen OffsetY-Werten erstellen
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

            // Speicheroptionen mit Wasserzeichen festlegen
            PdfSaveOptions options = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // Speichern mit Wasserzeichen-Versatz
            workbook.Save("WatermarkOffsetYDemo.pdf", options);
        }
    }
}
```

### Siehe auch

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


