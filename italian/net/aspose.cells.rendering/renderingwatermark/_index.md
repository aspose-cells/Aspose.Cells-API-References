---
title: "Classe RenderingWatermark"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Rendering.RenderingWatermark. Filigrana per il rendering"
type: docs
url: /it/net/aspose.cells.rendering/renderingwatermark/
---
## RenderingWatermark class

Filigrana per il rendering.

```csharp
public class RenderingWatermark
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [RenderingWatermark](renderingwatermark/#constructor)(byte[]) | Crea un'istanza di filigrana immagine. |
| [RenderingWatermark](renderingwatermark/#constructor_1)(string, RenderingFont) | Crea un'istanza di filigrana testo. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Font](../../aspose.cells.rendering/renderingwatermark/font/) { get; } | Ottiene il font della filigrana. |
| [HAlignment](../../aspose.cells.rendering/renderingwatermark/halignment/) { get; set; } | Ottiene o imposta l'allineamento orizzontale della filigrana rispetto alla pagina. |
| [Image](../../aspose.cells.rendering/renderingwatermark/image/) { get; } | Ottiene l'immagine della filigrana. |
| [IsBackground](../../aspose.cells.rendering/renderingwatermark/isbackground/) { get; set; } | Indica se la filigrana è posizionata dietro i contenuti della pagina. |
| [OffsetX](../../aspose.cells.rendering/renderingwatermark/offsetx/) { get; set; } | Ottiene o imposta il valore di offset a [`HAlignment`](./halignment/) |
| [OffsetY](../../aspose.cells.rendering/renderingwatermark/offsety/) { get; set; } | Ottiene o imposta il valore di offset a [`VAlignment`](./valignment/) |
| [Opacity](../../aspose.cells.rendering/renderingwatermark/opacity/) { get; set; } | Ottiene o imposta l'opacità della filigrana nell'intervallo [0, 1]. |
| [Rotation](../../aspose.cells.rendering/renderingwatermark/rotation/) { get; set; } | Ottiene o imposta la rotazione della filigrana in gradi. |
| [ScaleToPagePercent](../../aspose.cells.rendering/renderingwatermark/scaletopagepercent/) { get; set; } | Ottiene o imposta la scala relativa alla pagina di destinazione in percentuale. |
| [Text](../../aspose.cells.rendering/renderingwatermark/text/) { get; } | Ottiene il testo della filigrana. |
| [VAlignment](../../aspose.cells.rendering/renderingwatermark/valignment/) { get; set; } | Ottiene o imposta l'allineamento verticale della filigrana rispetto alla pagina. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing;

    public class RenderingWatermarkDemo
    {
        public static void RenderingWatermarkExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample worksheet.");

            // Crea un font per la filigrana
            RenderingFont font = new RenderingFont("Calibri", 68);
            font.Italic = true;
            font.Bold = true;
            font.Color = Color.Blue;

            // Crea una filigrana dal testo e dal font specificato
            RenderingWatermark watermark = new RenderingWatermark("Watermark", font);

            // Imposta le proprietà per la filigrana
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;
            watermark.Rotation = 30;
            watermark.Opacity = 0.6f;
            watermark.ScaleToPagePercent = 50;
            watermark.IsBackground = true;

            // Specifica la filigrana per il rendering in PDF
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // Salva la cartella di lavoro come PDF con la filigrana
            workbook.Save("output_watermark.pdf", options);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


