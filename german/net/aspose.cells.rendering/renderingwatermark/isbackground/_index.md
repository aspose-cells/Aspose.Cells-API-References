---
title: "RenderingWatermark.IsBackground"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RenderingWatermark-Eigenschaft. Gibt an, ob das Wasserzeichen hinter dem Seiteninhalt platziert wird"
type: docs
url: /de/net/aspose.cells.rendering/renderingwatermark/isbackground/
---
## RenderingWatermark.IsBackground property

Gibt an, ob das Wasserzeichen hinter dem Seiteninhalt platziert wird.

```csharp
public bool IsBackground { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Sample Content");

            // Erstelle ein Wasserzeichen mit IsBackground auf true gesetzt
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

            // Konfiguriere Speicheroptionen mit Wasserzeichen
            PdfSaveOptions options = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // Speichere mit Hintergrund-Wasserzeichen
            workbook.Save("WatermarkIsBackgroundDemo.pdf", options);
        }
    }
}
```

### Siehe auch

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


