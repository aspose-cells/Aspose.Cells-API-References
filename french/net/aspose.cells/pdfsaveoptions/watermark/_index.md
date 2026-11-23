---
title: "PdfSaveOptions.Watermark"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "PdfSaveOptions property. Obtient ou définit le filigrane à la sortie"
type: docs
url: /fr/net/aspose.cells/pdfsaveoptions/watermark/
---
## PdfSaveOptions.Watermark property

Obtient ou définit le filigrane à la sortie.

```csharp
public RenderingWatermark Watermark { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyWatermarkDemo
    {
        public static void Run()
        {
            // Créer un classeur avec 3 feuilles de calcul
            Workbook wb = new Workbook();
            wb.Worksheets[0].Cells["A1"].PutValue("Page1");
            int index = wb.Worksheets.Add();
            wb.Worksheets[index].Cells["A1"].PutValue("Page2");
            index = wb.Worksheets.Add();
            wb.Worksheets[index].Cells["A1"].PutValue("Page3");

            // Créer la police du filigrane
            RenderingFont font = new RenderingFont("Calibri", 68);
            font.Italic = true;
            font.Bold = true;
            font.Color = Color.Blue;

            // Créer un filigrane avec du texte et une police
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;
            watermark.Rotation = 45;
            watermark.Opacity = 0.3f;
            watermark.ScaleToPagePercent = 75;

            // Définir le filigrane dans les options d'enregistrement PDF
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // Enregistrer le classeur avec le filigrane
            wb.Save("output_watermark.pdf", options);
        }
    }
}
```

### Voir aussi

* class [RenderingWatermark](../../../aspose.cells.rendering/renderingwatermark/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


