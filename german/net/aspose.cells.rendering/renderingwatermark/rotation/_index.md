---
title: "RenderingWatermark.Rotation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RenderingWatermark-Eigenschaft. Gibt die Drehung des Wasserzeichens in Grad zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.rendering/renderingwatermark/rotation/
---
## RenderingWatermark.Rotation property

Liest oder setzt die Drehung des Wasserzeichens in Grad.

```csharp
public float Rotation { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data for watermark demo");

            // Erstelle Schriftart für Wasserzeichen
            RenderingFont font = new RenderingFont("Arial", 72);
            font.Color = Color.FromArgb(128, 0, 0, 255);
            font.Bold = true;

            // Erstelle Wasserzeichen mit Drehung
            RenderingWatermark watermark = new RenderingWatermark("ROTATED WATERMARK", font);
            watermark.Rotation = 45; // 45 degree rotation
            watermark.Opacity = 0.5f;
            watermark.IsBackground = true;

            // Setze PDF-Speicheroptionen mit Wasserzeichen
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // Speichere mit Wasserzeichen
            workbook.Save("WatermarkRotationDemo.pdf", options);
        }
    }
}
```

### Siehe auch

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


