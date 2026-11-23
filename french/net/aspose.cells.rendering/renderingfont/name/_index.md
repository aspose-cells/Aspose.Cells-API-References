---
title: "RenderingFont.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RenderingFont. Obtient le nom de la police"
type: docs
url: /fr/net/aspose.cells.rendering/renderingfont/name/
---
## RenderingFont.Name property

Obtient le nom de la police.

```csharp
public string Name { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingFontPropertyNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Créez les options d'enregistrement PDF
            PdfSaveOptions options = new PdfSaveOptions();

            // Créez la police de rendu initiale avec "Arial"
            RenderingFont fontArial = new RenderingFont("Arial", 16);
            Console.WriteLine("Initial font name: " + fontArial.Name);

            // Créez un filigrane avec la police initiale
            RenderingWatermark watermark = new RenderingWatermark("Confidential", fontArial);
            watermark.Opacity = 0.5f;
            watermark.Rotation = 45;
            options.Watermark = watermark;

            // Enregistrez avec le filigrane de police initiale
            workbook.Save("WatermarkInitial.pdf", options);

            // Créez une nouvelle police de rendu avec "Times New Roman"
            RenderingFont fontTimesNewRoman = new RenderingFont("Times New Roman", 16);
            Console.WriteLine("\nModified font name: " + fontTimesNewRoman.Name);

            // Mettez à jour le filigrane avec la nouvelle police
            RenderingWatermark updatedWatermark = new RenderingWatermark("Confidential", fontTimesNewRoman);
            updatedWatermark.Opacity = 0.5f;
            updatedWatermark.Rotation = 45;
            options.Watermark = updatedWatermark;

            // Enregistrez avec le filigrane de police modifié
            workbook.Save("WatermarkModified.pdf", options);
        }
    }
}
```

### Voir aussi

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


