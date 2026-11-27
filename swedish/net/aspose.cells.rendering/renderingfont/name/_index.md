---
title: "RenderingFont.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RenderingFont-egenskap. Hämtar namn på teckensnittet"
type: docs
url: /sv/net/aspose.cells.rendering/renderingfont/name/
---
## RenderingFont.Name property

Hämtar namn på typsnittet.

```csharp
public string Name { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Skapa PDF-sparalternativ
            PdfSaveOptions options = new PdfSaveOptions();

            // Skapa initial renderingsfont med "Arial"
            RenderingFont fontArial = new RenderingFont("Arial", 16);
            Console.WriteLine("Initial font name: " + fontArial.Name);

            // Skapa vattenstämpel med initialt teckensnitt
            RenderingWatermark watermark = new RenderingWatermark("Confidential", fontArial);
            watermark.Opacity = 0.5f;
            watermark.Rotation = 45;
            options.Watermark = watermark;

            // Spara med initial teckensnittsvattenstämpel
            workbook.Save("WatermarkInitial.pdf", options);

            // Skapa ny renderingsfont med "Times New Roman"
            RenderingFont fontTimesNewRoman = new RenderingFont("Times New Roman", 16);
            Console.WriteLine("\nModified font name: " + fontTimesNewRoman.Name);

            // Uppdatera vattenstämpel med nytt teckensnitt
            RenderingWatermark updatedWatermark = new RenderingWatermark("Confidential", fontTimesNewRoman);
            updatedWatermark.Opacity = 0.5f;
            updatedWatermark.Rotation = 45;
            options.Watermark = updatedWatermark;

            // Spara med modifierad teckensnittsvattenstämpel
            workbook.Save("WatermarkModified.pdf", options);
        }
    }
}
```

### Se även

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


