---
title: "RenderingWatermark.Image"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RenderingWatermark-egenskap. Hämtar bild av vattenstämpeln"
type: docs
url: /sv/net/aspose.cells.rendering/renderingwatermark/image/
---
## RenderingWatermark.Image property

Hämtar bilden av vattenstämpeln.

```csharp
public byte[] Image { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Läs in bilddata från fil
            byte[] originalImage = File.ReadAllBytes("watermark.png");

            // Skapa bildbaserad vattenstämpel med initial bild
            RenderingWatermark watermark = new RenderingWatermark(originalImage);
            Console.WriteLine("Initial image size: " + watermark.Image.Length + " bytes");

            // Ändra vattenstämpelns egenskaper
            watermark.Rotation = 45f;
            watermark.Opacity = 0.5f;
            watermark.ScaleToPagePercent = 75;
            watermark.IsBackground = true;
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;

            // Skapa PDF-sparalternativ med vattenstämpel
            PdfSaveOptions pdfOptions = new PdfSaveOptions();
            pdfOptions.Watermark = watermark; // Fixed property name

            // Spara till PDF med vattenstämpelutdata
            workbook.Save("WatermarkedOutput.pdf", pdfOptions);

            // Skapa ny vattenstämpel med annan bild
            byte[] updatedImage = File.ReadAllBytes("updated_watermark.png");
            RenderingWatermark newWatermark = new RenderingWatermark(updatedImage);
            Console.WriteLine("Updated image size: " + newWatermark.Image.Length + " bytes");

            // Spara med ny vattenstämpel
            pdfOptions.Watermark = newWatermark; // Fixed property name
            workbook.Save("UpdatedWatermark.pdf", pdfOptions);
        }
    }
}
```

### Se även

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


