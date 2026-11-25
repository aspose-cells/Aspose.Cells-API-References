---
title: "Class RenderingFont"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Rendering.RenderingFont class. Font per il rendering"
type: docs
url: /it/net/aspose.cells.rendering/renderingfont/
---
## RenderingFont class

Font per il rendering.

```csharp
public class RenderingFont
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [RenderingFont](renderingfont/)(string, float) | Inizializza una nuova istanza di `RenderingFont` |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Bold](../../aspose.cells.rendering/renderingfont/bold/) { get; set; } | Ottiene o imposta il grassetto per il font. |
| [Color](../../aspose.cells.rendering/renderingfont/color/) { get; set; } | Ottiene o imposta il colore per il font. |
| [Italic](../../aspose.cells.rendering/renderingfont/italic/) { get; set; } | Ottiene o imposta il corsivo per il font. |
| [Name](../../aspose.cells.rendering/renderingfont/name/) { get; } | Ottiene il nome del font. |
| [Size](../../aspose.cells.rendering/renderingfont/size/) { get; } | Ottiene la dimensione del font in punti. |

### Esempi

```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontDemo
    {
        public static void RenderingFontExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            sheet.Cells["A1"].PutValue("Hello World!");

            // Crea un oggetto RenderingFont
            RenderingFont renderingFont = new RenderingFont("Arial", 12)
            {
                Bold = true,
                Italic = true,
                Color = Color.Blue
            };

            // Crea un oggetto RenderingWatermark usando il RenderingFont
            RenderingWatermark watermark = new RenderingWatermark("Sample Watermark", renderingFont)
            {
                Rotation = 45,
                ScaleToPagePercent = 100,
                Opacity = 0.5f,
                IsBackground = true,
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                OffsetX = 0,
                OffsetY = 0
            };

            // Crea PdfSaveOptions e imposta la filigrana
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions
            {
                Watermark = watermark,
                EmbedStandardWindowsFonts = true,
                CalculateFormula = true,
                ExportDocumentStructure = true,
                DisplayDocTitle = true
            };

            // Salva la cartella di lavoro in PDF con la filigrana
            workbook.Save("RenderingFontExample.pdf", pdfSaveOptions);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


