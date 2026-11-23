---
title: "RenderingFont.Bold"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RenderingFont. Obtient ou définit le gras pour la police"
type: docs
url: /fr/net/aspose.cells.rendering/renderingfont/bold/
---
## RenderingFont.Bold property

Obtient ou définit le gras pour la police.

```csharp
public bool Bold { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontPropertyBoldDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Bold Font Example");

            // Créer un style pour la cellule
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            worksheet.Cells["A1"].SetStyle(style);

            // Créer des options d'enregistrement PDF avec filigrane démontrant une police en gras
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Créer une police de rendu avec la propriété gras
            RenderingFont font = new RenderingFont("Arial", 36)
            {
                Bold = true,
                Color = System.Drawing.Color.Red
            };
            
            // Créer un filigrane avec une police en gras
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font)
            {
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                Opacity = 0.3f
            };
            pdfSaveOptions.Watermark = watermark;

            // Enregistrez le classeur
            workbook.Save("BoldFontExample.pdf", pdfSaveOptions);
        }
    }
}
```

### Voir aussi

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


