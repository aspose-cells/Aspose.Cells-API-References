---
title: "RenderingFont.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RenderingFont. Ottiene il nome del carattere"
type: docs
url: /it/net/aspose.cells.rendering/renderingfont/name/
---
## RenderingFont.Name property

Ottiene il nome del font.

```csharp
public string Name { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingFontPropertyNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Crea le opzioni di salvataggio PDF
            PdfSaveOptions options = new PdfSaveOptions();

            // Crea il carattere di rendering iniziale con "Arial"
            RenderingFont fontArial = new RenderingFont("Arial", 16);
            Console.WriteLine("Initial font name: " + fontArial.Name);

            // Crea una filigrana con il carattere iniziale
            RenderingWatermark watermark = new RenderingWatermark("Confidential", fontArial);
            watermark.Opacity = 0.5f;
            watermark.Rotation = 45;
            options.Watermark = watermark;

            // Salva con la filigrana del carattere iniziale
            workbook.Save("WatermarkInitial.pdf", options);

            // Crea un nuovo carattere di rendering con "Times New Roman"
            RenderingFont fontTimesNewRoman = new RenderingFont("Times New Roman", 16);
            Console.WriteLine("\nModified font name: " + fontTimesNewRoman.Name);

            // Aggiorna la filigrana con il nuovo carattere
            RenderingWatermark updatedWatermark = new RenderingWatermark("Confidential", fontTimesNewRoman);
            updatedWatermark.Opacity = 0.5f;
            updatedWatermark.Rotation = 45;
            options.Watermark = updatedWatermark;

            // Salva con la filigrana del carattere modificato
            workbook.Save("WatermarkModified.pdf", options);
        }
    }
}
```

### Vedi anche

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


