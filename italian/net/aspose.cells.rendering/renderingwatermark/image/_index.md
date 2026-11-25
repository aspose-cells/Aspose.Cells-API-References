---
title: "RenderingWatermark.Image"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RenderingWatermark. Ottiene l'immagine della filigrana"
type: docs
url: /it/net/aspose.cells.rendering/renderingwatermark/image/
---
## RenderingWatermark.Image property

Ottiene l'immagine della filigrana.

```csharp
public byte[] Image { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System.IO;

    public class RenderingWatermarkPropertyImageDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Carica i dati immagine dal file
            byte[] originalImage = File.ReadAllBytes("watermark.png");

            // Crea una filigrana basata su immagine con l'immagine iniziale
            RenderingWatermark watermark = new RenderingWatermark(originalImage);
            Console.WriteLine("Initial image size: " + watermark.Image.Length + " bytes");

            // Modifica le proprietà della filigrana
            watermark.Rotation = 45f;
            watermark.Opacity = 0.5f;
            watermark.ScaleToPagePercent = 75;
            watermark.IsBackground = true;
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;

            // Crea opzioni di salvataggio PDF con filigrana
            PdfSaveOptions pdfOptions = new PdfSaveOptions();
            pdfOptions.Watermark = watermark; // Fixed property name

            // Salva in PDF con output filigranato
            workbook.Save("WatermarkedOutput.pdf", pdfOptions);

            // Crea una nuova filigrana con immagine diversa
            byte[] updatedImage = File.ReadAllBytes("updated_watermark.png");
            RenderingWatermark newWatermark = new RenderingWatermark(updatedImage);
            Console.WriteLine("Updated image size: " + newWatermark.Image.Length + " bytes");

            // Salva con la nuova filigrana
            pdfOptions.Watermark = newWatermark; // Fixed property name
            workbook.Save("UpdatedWatermark.pdf", pdfOptions);
        }
    }
}
```

### Vedi anche

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


