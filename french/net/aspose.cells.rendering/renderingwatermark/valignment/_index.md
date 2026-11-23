---
title: "RenderingWatermark.VAlignment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RenderingWatermark. Obtient ou définit l'alignement vertical du filigrane par rapport à la page"
type: docs
url: /fr/net/aspose.cells.rendering/renderingwatermark/valignment/
---
## RenderingWatermark.VAlignment property

Obtient ou définit l'alignement vertical du filigrane par rapport à la page.

```csharp
public TextAlignmentType VAlignment { get; set; }
```

### Remarques

Seuls Top, Center, Bottom sont valides. La valeur par défaut est Top.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyVAlignmentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Watermark VAlignment Demo");

            // Créez les options d'enregistrement PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Créer et configurer un filigrane avec différents paramètres VAlignment
            RenderingFont font = new RenderingFont("Arial", 48)
            {
                Bold = true,
                Color = System.Drawing.Color.Red
            };

            // Créer un filigrane avec l'alignement vertical défini sur Center
            RenderingWatermark watermark = new RenderingWatermark("CENTER ALIGNED", font)
            {
                VAlignment = TextAlignmentType.Center,
                HAlignment = TextAlignmentType.Center,
                Opacity = 0.5f
            };
            pdfSaveOptions.Watermark = watermark;

            // Enregistrer le classeur avec filigrane
            workbook.Save("WatermarkVAlignmentDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Voir aussi

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


