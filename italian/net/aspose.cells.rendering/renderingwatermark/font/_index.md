---
title: "RenderingWatermark.Font"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RenderingWatermark. Ottiene il font della filigrana"
type: docs
url: /it/net/aspose.cells.rendering/renderingwatermark/font/
---
## RenderingWatermark.Font property

Ottiene il font della filigrana.

```csharp
public RenderingFont Font { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingWatermarkPropertyFontDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Crea un font di rendering e imposta le proprietà iniziali
            RenderingFont font = new RenderingFont("Arial", 24);
            
            // Crea una filigrana di testo con il font di rendering
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
            
            // Visualizza le proprietà del font iniziali
            Console.WriteLine("Initial Font Name: " + watermark.Font.Name);
            Console.WriteLine("Initial Font Size: " + watermark.Font.Size);
            Console.WriteLine("Initial Bold Status: " + watermark.Font.Bold);
            
            // Modifica le proprietà del font tramite il riferimento RenderingFont
            font.Bold = true;
            
            // Visualizza le proprietà del font aggiornate dalla filigrana
            Console.WriteLine("\nUpdated Font Name: " + watermark.Font.Name);
            Console.WriteLine("Updated Font Size: " + watermark.Font.Size);
            Console.WriteLine("Updated Bold Status: " + watermark.Font.Bold);
            
            // Configura le proprietà di visualizzazione della filigrana
            watermark.Opacity = 0.5f;
            watermark.Rotation = 45;
            watermark.IsBackground = true;
            
            // Crea le opzioni di salvataggio PDF e assegna la filigrana
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.Watermark = watermark;
            
            // Salva la cartella di lavoro con PDF filigranato per mostrare le modifiche al font
            workbook.Save("RenderingWatermarkFontDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Vedi anche

* class [RenderingFont](../../renderingfont/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


