---
title: "RenderingFont.Size"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RenderingFont. Ottiene la dimensione del carattere in punti"
type: docs
url: /it/net/aspose.cells.rendering/renderingfont/size/
---
## RenderingFont.Size property

Ottiene la dimensione del font in punti.

```csharp
public float Size { get; }
```

### Esempi

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
            
            // Crea il carattere iniziale e dimostra la lettura della proprietà Size
            RenderingFont smallFont = new RenderingFont("Arial", 12);
            Console.WriteLine("Initial font size: " + smallFont.Size);

            // Crea una filigrana con la dimensione iniziale del carattere
            PdfSaveOptions optionsSmall = new PdfSaveOptions
            {
                Watermark = new RenderingWatermark("CONFIDENTIAL", smallFont)
            };
            workbook.Save("SmallWatermark.pdf", optionsSmall);

            // Crea un nuovo carattere con dimensione più grande
            RenderingFont largeFont = new RenderingFont("Arial", 24);
            Console.WriteLine("Modified font size: " + largeFont.Size);

            // Crea una filigrana con dimensione del carattere più grande
            PdfSaveOptions optionsLarge = new PdfSaveOptions
            {
                Watermark = new RenderingWatermark("CONFIDENTIAL", largeFont)
            };
            workbook.Save("LargeWatermark.pdf", optionsLarge);
        }
    }
}
```

### Vedi anche

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


