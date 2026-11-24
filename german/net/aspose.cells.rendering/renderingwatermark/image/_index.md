---
title: "RenderingWatermark.Image"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RenderingWatermark-Eigenschaft. Gibt das Bild des Wasserzeichens zurück"
type: docs
url: /de/net/aspose.cells.rendering/renderingwatermark/image/
---
## RenderingWatermark.Image property

Liest das Bild des Wasserzeichens.

```csharp
public byte[] Image { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lade Bilddaten aus Datei
            byte[] originalImage = File.ReadAllBytes("watermark.png");

            // Erstelle bildbasiertes Wasserzeichen mit dem Ausgangsbild
            RenderingWatermark watermark = new RenderingWatermark(originalImage);
            Console.WriteLine("Initial image size: " + watermark.Image.Length + " bytes");

            // Ändere die Wasserzeichen-Eigenschaften
            watermark.Rotation = 45f;
            watermark.Opacity = 0.5f;
            watermark.ScaleToPagePercent = 75;
            watermark.IsBackground = true;
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;

            // Erstelle PDF-Speicheroptionen mit Wasserzeichen
            PdfSaveOptions pdfOptions = new PdfSaveOptions();
            pdfOptions.Watermark = watermark; // Fixed property name

            // Speichere als PDF mit wasserzeichenhaltigem Ergebnis
            workbook.Save("WatermarkedOutput.pdf", pdfOptions);

            // Erstelle ein neues Wasserzeichen mit anderem Bild
            byte[] updatedImage = File.ReadAllBytes("updated_watermark.png");
            RenderingWatermark newWatermark = new RenderingWatermark(updatedImage);
            Console.WriteLine("Updated image size: " + newWatermark.Image.Length + " bytes");

            // Speichere mit neuem Wasserzeichen
            pdfOptions.Watermark = newWatermark; // Fixed property name
            workbook.Save("UpdatedWatermark.pdf", pdfOptions);
        }
    }
}
```

### Siehe auch

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


