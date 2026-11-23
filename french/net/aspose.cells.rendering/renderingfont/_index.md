---
title: "Class RenderingFont"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Rendering.RenderingFont class. Police pour le rendu"
type: docs
url: /fr/net/aspose.cells.rendering/renderingfont/
---
## RenderingFont class

Police pour le rendu.

```csharp
public class RenderingFont
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [RenderingFont](renderingfont/)(string, float) | Initialise une nouvelle instance de `RenderingFont` |

## Propriétés

| Nom | Description |
| --- | --- |
| [Bold](../../aspose.cells.rendering/renderingfont/bold/) { get; set; } | Obtient ou définit le gras pour la police. |
| [Color](../../aspose.cells.rendering/renderingfont/color/) { get; set; } | Obtient ou définit la couleur pour la police. |
| [Italic](../../aspose.cells.rendering/renderingfont/italic/) { get; set; } | Obtient ou définit l'italique pour la police. |
| [Name](../../aspose.cells.rendering/renderingfont/name/) { get; } | Obtient le nom de la police. |
| [Size](../../aspose.cells.rendering/renderingfont/size/) { get; } | Obtient la taille de la police en points. |

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontDemo
    {
        public static void RenderingFontExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Hello World!");

            // Crée un objet RenderingFont
            RenderingFont renderingFont = new RenderingFont("Arial", 12)
            {
                Bold = true,
                Italic = true,
                Color = Color.Blue
            };

            // Crée un objet RenderingWatermark en utilisant le RenderingFont
            RenderingWatermark watermark = new RenderingWatermark("Sample Watermark", renderingFont)
            {
                Rotation = 45,
                ScaleToPagePercent = 100,
                Opacity = 0.5f,
                IsBackground = true,
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                OffsetX = 0,
                OffsetY = 0
            };

            // Crée PdfSaveOptions et définit le filigrane
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions
            {
                Watermark = watermark,
                EmbedStandardWindowsFonts = true,
                CalculateFormula = true,
                ExportDocumentStructure = true,
                DisplayDocTitle = true
            };

            // Enregistre le classeur au format PDF avec le filigrane
            workbook.Save("RenderingFontExample.pdf", pdfSaveOptions);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


