---
title: "RenderingWatermark.HAlignment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RenderingWatermark property. Gibt die horizontale Ausrichtung des Wasserzeichens zur Seite zurück oder setzt sie"
type: docs
url: /de/net/aspose.cells.rendering/renderingwatermark/halignment/
---
## RenderingWatermark.HAlignment property

Liest oder setzt die horizontale Ausrichtung des Wasserzeichens zur Seite.

```csharp
public TextAlignmentType HAlignment { get; set; }
```

### Hinweise

Nur Links, Mitte, Rechts ist gültig. Standard ist Links.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyHAlignmentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Watermark HAlignment Demo");

            // PDF-Speicheroptionen erstellen
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Erstelle und konfiguriere Wasserzeichen mit verschiedenen HAlignment-Einstellungen
            RenderingFont font = new RenderingFont("Arial", 48)
            {
                Bold = true,
                Color = System.Drawing.Color.Blue
            };

            // Erstelle Wasserzeichen mit Center-Ausrichtung
            RenderingWatermark watermark = new RenderingWatermark("CENTER ALIGNED", font)
            {
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                Opacity = 0.5f
            };
            pdfSaveOptions.Watermark = watermark;

            // Speichere mit zentriert ausgerichtem Wasserzeichen
            workbook.Save("WatermarkCenterAlignment.pdf", pdfSaveOptions);

            // Ändere zu Links-Ausrichtung
            watermark.HAlignment = TextAlignmentType.Left;
            workbook.Save("WatermarkLeftAlignment.pdf", pdfSaveOptions);

            // Ändere zu Rechts-Ausrichtung
            watermark.HAlignment = TextAlignmentType.Right;
            workbook.Save("WatermarkRightAlignment.pdf", pdfSaveOptions);
        }
    }
}
```

### Siehe auch

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


