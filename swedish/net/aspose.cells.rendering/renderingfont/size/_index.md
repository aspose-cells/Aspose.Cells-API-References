---
title: "RenderingFont.Size"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RenderingFont-egenskap. Hämtar storlek på teckensnittet i punkter"
type: docs
url: /sv/net/aspose.cells.rendering/renderingfont/size/
---
## RenderingFont.Size property

Hämtar storlek på typsnittet i punkter.

```csharp
public float Size { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingFontPropertySizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Skapa initialt teckensnitt och demonstrera läsning av Size-egenskapen
            RenderingFont smallFont = new RenderingFont("Arial", 12);
            Console.WriteLine("Initial font size: " + smallFont.Size);

            // Skapa vattenstämpel med initial teckensnittsstorlek
            PdfSaveOptions optionsSmall = new PdfSaveOptions
            {
                Watermark = new RenderingWatermark("CONFIDENTIAL", smallFont)
            };
            workbook.Save("SmallWatermark.pdf", optionsSmall);

            // Skapa nytt teckensnitt med större storlek
            RenderingFont largeFont = new RenderingFont("Arial", 24);
            Console.WriteLine("Modified font size: " + largeFont.Size);

            // Skapa vattenstämpel med större teckensnittsstorlek
            PdfSaveOptions optionsLarge = new PdfSaveOptions
            {
                Watermark = new RenderingWatermark("CONFIDENTIAL", largeFont)
            };
            workbook.Save("LargeWatermark.pdf", optionsLarge);
        }
    }
}
```

### Se även

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


