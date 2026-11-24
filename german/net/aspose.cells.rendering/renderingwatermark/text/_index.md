---
title: "RenderingWatermark.Text"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RenderingWatermark-Eigenschaft. Gibt den Text des Wasserzeichens zurück"
type: docs
url: /de/net/aspose.cells.rendering/renderingwatermark/text/
---
## RenderingWatermark.Text property

Liest den Text des Wasserzeichens.

```csharp
public string Text { get; }
```

### Beispiele

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

            // Erstelle Rendering-Schriftart für Wasserzeichentext
            RenderingFont font = new RenderingFont("Arial", 36);

            // Initialisiere Textwasserzeichen mit Schriftkonfiguration
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);

            // Zeige aktuellen Wasserzeichentext an
            Console.WriteLine("Watermark Text: " + watermark.Text);

            // Konfiguriere Aussehen des Wasserzeichens
            watermark.Rotation = 45f;
            watermark.Opacity = 0.3f;
            watermark.IsBackground = true;
            watermark.ScaleToPagePercent = 150;

            // Wende Wasserzeichen auf PDF-Speicheroptionen an
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark; // Fixed property name

            // Speichere als PDF, um Wasserzeicheneffekte zu visualisieren
            workbook.Save("WatermarkDemo.pdf", options);
        }
    }
}
```

### Siehe auch

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


