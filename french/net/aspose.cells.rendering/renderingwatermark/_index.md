---
title: "Classe RenderingWatermark"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Rendering.RenderingWatermark. Filigrane pour le rendu"
type: docs
url: /fr/net/aspose.cells.rendering/renderingwatermark/
---
## RenderingWatermark class

Filigrane pour le rendu.

```csharp
public class RenderingWatermark
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [RenderingWatermark](renderingwatermark/#constructor)(byte[]) | Crée une instance de filigrane image. |
| [RenderingWatermark](renderingwatermark/#constructor_1)(string, RenderingFont) | Crée une instance de filigrane texte. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Font](../../aspose.cells.rendering/renderingwatermark/font/) { get; } | Obtient la police du filigrane. |
| [HAlignment](../../aspose.cells.rendering/renderingwatermark/halignment/) { get; set; } | Obtient ou définit l'alignement horizontal du filigrane par rapport à la page. |
| [Image](../../aspose.cells.rendering/renderingwatermark/image/) { get; } | Obtient l'image du filigrane. |
| [IsBackground](../../aspose.cells.rendering/renderingwatermark/isbackground/) { get; set; } | Indique si le filigrane est placé derrière le contenu de la page. |
| [OffsetX](../../aspose.cells.rendering/renderingwatermark/offsetx/) { get; set; } | Obtient ou définit la valeur de décalage pour [`HAlignment`](./halignment/) |
| [OffsetY](../../aspose.cells.rendering/renderingwatermark/offsety/) { get; set; } | Obtient ou définit la valeur de décalage pour [`VAlignment`](./valignment/) |
| [Opacity](../../aspose.cells.rendering/renderingwatermark/opacity/) { get; set; } | Obtient ou définit l'opacité du filigrane dans la plage [0, 1]. |
| [Rotation](../../aspose.cells.rendering/renderingwatermark/rotation/) { get; set; } | Obtient ou définit la roation du filigrane en degrés. |
| [ScaleToPagePercent](../../aspose.cells.rendering/renderingwatermark/scaletopagepercent/) { get; set; } | Obtient ou définit l'échelle relative à la page cible en pourcentage. |
| [Text](../../aspose.cells.rendering/renderingwatermark/text/) { get; } | Obtient le texte du filigrane. |
| [VAlignment](../../aspose.cells.rendering/renderingwatermark/valignment/) { get; set; } | Obtient ou définit l'alignement vertical du filigrane par rapport à la page. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing;

    public class RenderingWatermarkDemo
    {
        public static void RenderingWatermarkExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample worksheet.");

            // Crée une police pour le filigrane
            RenderingFont font = new RenderingFont("Calibri", 68);
            font.Italic = true;
            font.Bold = true;
            font.Color = Color.Blue;

            // Crée un filigrane à partir du texte et de la police spécifiée
            RenderingWatermark watermark = new RenderingWatermark("Watermark", font);

            // Définit les propriétés du filigrane
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;
            watermark.Rotation = 30;
            watermark.Opacity = 0.6f;
            watermark.ScaleToPagePercent = 50;
            watermark.IsBackground = true;

            // Spécifie le filigrane pour le rendu en PDF
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // Enregistrez le classeur au format PDF avec le filigrane
            workbook.Save("output_watermark.pdf", options);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


