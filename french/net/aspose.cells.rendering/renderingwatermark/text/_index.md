---
title: "RenderingWatermark.Text"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RenderingWatermark. Obtient le texte du filigrane"
type: docs
url: /fr/net/aspose.cells.rendering/renderingwatermark/text/
---
## RenderingWatermark.Text property

Obtient le texte du filigrane.

```csharp
public string Text { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingWatermarkPropertyTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une police de rendu pour le texte du filigrane
            RenderingFont font = new RenderingFont("Arial", 36);

            // Initialiser le filigrane texte avec la configuration de police
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);

            // Afficher le texte actuel du filigrane
            Console.WriteLine("Watermark Text: " + watermark.Text);

            // Configurer l'apparence du filigrane
            watermark.Rotation = 45f;
            watermark.Opacity = 0.3f;
            watermark.IsBackground = true;
            watermark.ScaleToPagePercent = 150;

            // Appliquer le filigrane aux options d'enregistrement PDF
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark; // Fixed property name

            // Enregistrer en PDF pour visualiser les effets du filigrane
            workbook.Save("WatermarkDemo.pdf", options);
        }
    }
}
```

### Voir aussi

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


