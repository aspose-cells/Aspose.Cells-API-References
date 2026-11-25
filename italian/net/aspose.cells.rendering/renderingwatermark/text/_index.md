---
title: "RenderingWatermark.Text"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RenderingWatermark. Ottiene il testo della filigrana"
type: docs
url: /it/net/aspose.cells.rendering/renderingwatermark/text/
---
## RenderingWatermark.Text property

Ottiene il testo della filigrana.

```csharp
public string Text { get; }
```

### Esempi

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

            // Crea il carattere di rendering per il testo della filigrana
            RenderingFont font = new RenderingFont("Arial", 36);

            // Inizializza la filigrana di testo con la configurazione del carattere
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);

            // Visualizza il testo corrente della filigrana
            Console.WriteLine("Watermark Text: " + watermark.Text);

            // Configura l'aspetto della filigrana
            watermark.Rotation = 45f;
            watermark.Opacity = 0.3f;
            watermark.IsBackground = true;
            watermark.ScaleToPagePercent = 150;

            // Applica la filigrana alle opzioni di salvataggio PDF
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark; // Fixed property name

            // Salva in PDF per visualizzare gli effetti della filigrana
            workbook.Save("WatermarkDemo.pdf", options);
        }
    }
}
```

### Vedi anche

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


