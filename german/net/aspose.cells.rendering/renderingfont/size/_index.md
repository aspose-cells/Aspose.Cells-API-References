---
title: "RenderingFont.Size"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RenderingFont-Eigenschaft. Gibt die Größe der Schriftart in Punkten zurück."
type: docs
url: /de/net/aspose.cells.rendering/renderingfont/size/
---
## RenderingFont.Size property

Liest die Größe der Schriftart in Punkten.

```csharp
public float Size { get; }
```

### Beispiele

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
            
            // Initiale Schriftart erstellen und das Auslesen der Size‑Eigenschaft demonstrieren.
            RenderingFont smallFont = new RenderingFont("Arial", 12);
            Console.WriteLine("Initial font size: " + smallFont.Size);

            // Wasserzeichen mit initialer Schriftgröße erstellen.
            PdfSaveOptions optionsSmall = new PdfSaveOptions
            {
                Watermark = new RenderingWatermark("CONFIDENTIAL", smallFont)
            };
            workbook.Save("SmallWatermark.pdf", optionsSmall);

            // Neue Schriftart mit größerer Größe erstellen.
            RenderingFont largeFont = new RenderingFont("Arial", 24);
            Console.WriteLine("Modified font size: " + largeFont.Size);

            // Wasserzeichen mit größerer Schriftgröße erstellen
            PdfSaveOptions optionsLarge = new PdfSaveOptions
            {
                Watermark = new RenderingWatermark("CONFIDENTIAL", largeFont)
            };
            workbook.Save("LargeWatermark.pdf", optionsLarge);
        }
    }
}
```

### Siehe auch

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


