---
title: "RenderingWatermark.Image"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RenderingWatermark. Obtient l'image du filigrane"
type: docs
url: /fr/net/aspose.cells.rendering/renderingwatermark/image/
---
## RenderingWatermark.Image property

Obtient l'image du filigrane.

```csharp
public byte[] Image { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System.IO;

    public class RenderingWatermarkPropertyImageDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Charger les données d'image depuis le fichier
            byte[] originalImage = File.ReadAllBytes("watermark.png");

            // Créer un filigrane basé sur une image avec l'image initiale
            RenderingWatermark watermark = new RenderingWatermark(originalImage);
            Console.WriteLine("Initial image size: " + watermark.Image.Length + " bytes");

            // Modifier les propriétés du filigrane
            watermark.Rotation = 45f;
            watermark.Opacity = 0.5f;
            watermark.ScaleToPagePercent = 75;
            watermark.IsBackground = true;
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;

            // Créer des options d'enregistrement PDF avec filigrane
            PdfSaveOptions pdfOptions = new PdfSaveOptions();
            pdfOptions.Watermark = watermark; // Fixed property name

            // Enregistrer en PDF avec une sortie filigranée
            workbook.Save("WatermarkedOutput.pdf", pdfOptions);

            // Créer un nouveau filigrane avec une image différente
            byte[] updatedImage = File.ReadAllBytes("updated_watermark.png");
            RenderingWatermark newWatermark = new RenderingWatermark(updatedImage);
            Console.WriteLine("Updated image size: " + newWatermark.Image.Length + " bytes");

            // Enregistrer avec le nouveau filigrane
            pdfOptions.Watermark = newWatermark; // Fixed property name
            workbook.Save("UpdatedWatermark.pdf", pdfOptions);
        }
    }
}
```

### Voir aussi

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


