---
title: "PdfSaveOptions.Watermark"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PdfSaveOptions property. Ottiene o imposta la filigrana da esportare"
type: docs
url: /it/net/aspose.cells/pdfsaveoptions/watermark/
---
## PdfSaveOptions.Watermark property

Ottiene o imposta la filigrana in output.

```csharp
public RenderingWatermark Watermark { get; set; }
```

### Esempi

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
            // Crea una cartella di lavoro con 3 fogli di lavoro
            Workbook wb = new Workbook();
            wb.Worksheets[0].Cells["A1"].PutValue("Page1");
            int index = wb.Worksheets.Add();
            wb.Worksheets[index].Cells["A1"].PutValue("Page2");
            index = wb.Worksheets.Add();
            wb.Worksheets[index].Cells["A1"].PutValue("Page3");

            // Crea il carattere della filigrana
            RenderingFont font = new RenderingFont("Calibri", 68);
            font.Italic = true;
            font.Bold = true;
            font.Color = Color.Blue;

            // Crea una filigrana con testo e carattere
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;
            watermark.Rotation = 45;
            watermark.Opacity = 0.3f;
            watermark.ScaleToPagePercent = 75;

            // Imposta la filigrana nelle opzioni di salvataggio PDF
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // Salva la cartella di lavoro con filigrana
            wb.Save("output_watermark.pdf", options);
        }
    }
}
```

### Vedi anche

* class [RenderingWatermark](../../../aspose.cells.rendering/renderingwatermark/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


