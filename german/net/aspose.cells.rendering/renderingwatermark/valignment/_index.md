---
title: "RenderingWatermark.VAlignment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RenderingWatermark-Eigenschaft. Gibt die vertikale Ausrichtung des Wasserzeichens zur Seite zurück oder legt sie fest."
type: docs
url: /de/net/aspose.cells.rendering/renderingwatermark/valignment/
---
## RenderingWatermark.VAlignment property

Liest oder setzt die vertikale Ausrichtung des Wasserzeichens zur Seite.

```csharp
public TextAlignmentType VAlignment { get; set; }
```

### Hinweise

Nur Top, Center, Bottom sind gültig. Standard ist Top.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyVAlignmentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Watermark VAlignment Demo");

            // PDF-Speicheroptionen erstellen
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Erstellen und konfigurieren Sie ein Wasserzeichen mit verschiedenen VAlignment-Einstellungen.
            RenderingFont font = new RenderingFont("Arial", 48)
            {
                Bold = true,
                Color = System.Drawing.Color.Red
            };

            // Erstellen Sie ein Wasserzeichen mit vertikaler Ausrichtung auf Center gesetzt.
            RenderingWatermark watermark = new RenderingWatermark("CENTER ALIGNED", font)
            {
                VAlignment = TextAlignmentType.Center,
                HAlignment = TextAlignmentType.Center,
                Opacity = 0.5f
            };
            pdfSaveOptions.Watermark = watermark;

            // Speichere die Arbeitsmappe mit Wasserzeichen
            workbook.Save("WatermarkVAlignmentDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Siehe auch

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


