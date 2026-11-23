---
title: "RenderingFont.Size"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RenderingFont. Obtient la taille de la police en points"
type: docs
url: /fr/net/aspose.cells.rendering/renderingfont/size/
---
## RenderingFont.Size property

Obtient la taille de la police en points.

```csharp
public float Size { get; }
```

### Exemples

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
            
            // Créez la police initiale et démontrez la lecture de la propriété Size
            RenderingFont smallFont = new RenderingFont("Arial", 12);
            Console.WriteLine("Initial font size: " + smallFont.Size);

            // Créez un filigrane avec la taille de police initiale
            PdfSaveOptions optionsSmall = new PdfSaveOptions
            {
                Watermark = new RenderingWatermark("CONFIDENTIAL", smallFont)
            };
            workbook.Save("SmallWatermark.pdf", optionsSmall);

            // Créez une nouvelle police avec une taille plus grande
            RenderingFont largeFont = new RenderingFont("Arial", 24);
            Console.WriteLine("Modified font size: " + largeFont.Size);

            // Créez un filigrane avec une taille de police plus grande
            PdfSaveOptions optionsLarge = new PdfSaveOptions
            {
                Watermark = new RenderingWatermark("CONFIDENTIAL", largeFont)
            };
            workbook.Save("LargeWatermark.pdf", optionsLarge);
        }
    }
}
```

### Voir aussi

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


