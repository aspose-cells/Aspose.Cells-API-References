---
title: "PdfSaveOptions.Watermark"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSaveOptions-Eigenschaft. Gibt das Wasserzeichen zurück oder legt es für die Ausgabe fest"
type: docs
url: /de/net/aspose.cells/pdfsaveoptions/watermark/
---
## PdfSaveOptions.Watermark property

Liest oder setzt das Wasserzeichen für die Ausgabe.

```csharp
public RenderingWatermark Watermark { get; set; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyWatermarkDemo
    {
        public static void Run()
        {
            // Erstellen Sie ein Arbeitsbuch mit 3 Arbeitsblättern
            Workbook wb = new Workbook();
            wb.Worksheets[0].Cells["A1"].PutValue("Page1");
            int index = wb.Worksheets.Add();
            wb.Worksheets[index].Cells["A1"].PutValue("Page2");
            index = wb.Worksheets.Add();
            wb.Worksheets[index].Cells["A1"].PutValue("Page3");

            // Erstellen Sie die Wasserzeichen-Schriftart
            RenderingFont font = new RenderingFont("Calibri", 68);
            font.Italic = true;
            font.Bold = true;
            font.Color = Color.Blue;

            // Wasserzeichen mit Text und Schriftart erstellen
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;
            watermark.Rotation = 45;
            watermark.Opacity = 0.3f;
            watermark.ScaleToPagePercent = 75;

            // Wasserzeichen in PDF‑Speicheroptionen festlegen
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // Arbeitsmappe mit Wasserzeichen speichern
            wb.Save("output_watermark.pdf", options);
        }
    }
}
```

### Siehe auch

* class [RenderingWatermark](../../../aspose.cells.rendering/renderingwatermark/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


