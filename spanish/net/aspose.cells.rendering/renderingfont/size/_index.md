---
title: "RenderingFont.Size"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RenderingFont. Obtiene el tamaño de la fuente en puntos"
type: docs
url: /es/net/aspose.cells.rendering/renderingfont/size/
---
## RenderingFont.Size property

Obtiene el tamaño de la fuente en puntos.

```csharp
public float Size { get; }
```

### Ejemplos

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
            
            // Crea una fuente inicial y demuestra la lectura de la propiedad Size
            RenderingFont smallFont = new RenderingFont("Arial", 12);
            Console.WriteLine("Initial font size: " + smallFont.Size);

            // Crea una marca de agua con el tamaño de fuente inicial
            PdfSaveOptions optionsSmall = new PdfSaveOptions
            {
                Watermark = new RenderingWatermark("CONFIDENTIAL", smallFont)
            };
            workbook.Save("SmallWatermark.pdf", optionsSmall);

            // Crea una nueva fuente con un tamaño más grande
            RenderingFont largeFont = new RenderingFont("Arial", 24);
            Console.WriteLine("Modified font size: " + largeFont.Size);

            // Crea una marca de agua con un tamaño de fuente más grande
            PdfSaveOptions optionsLarge = new PdfSaveOptions
            {
                Watermark = new RenderingWatermark("CONFIDENTIAL", largeFont)
            };
            workbook.Save("LargeWatermark.pdf", optionsLarge);
        }
    }
}
```

### Ver también

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


