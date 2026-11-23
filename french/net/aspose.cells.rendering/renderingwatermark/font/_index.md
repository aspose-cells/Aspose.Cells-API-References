---
title: "RenderingWatermark.Font"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RenderingWatermark. Obtient la police du filigrane"
type: docs
url: /fr/net/aspose.cells.rendering/renderingwatermark/font/
---
## RenderingWatermark.Font property

Obtient la police du filigrane.

```csharp
public RenderingFont Font { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingWatermarkPropertyFontDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Créer une police de rendu et définir les propriétés initiales
            RenderingFont font = new RenderingFont("Arial", 24);
            
            // Créer un filigrane texte avec la police de rendu
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
            
            // Afficher les propriétés de police initiales
            Console.WriteLine("Initial Font Name: " + watermark.Font.Name);
            Console.WriteLine("Initial Font Size: " + watermark.Font.Size);
            Console.WriteLine("Initial Bold Status: " + watermark.Font.Bold);
            
            // Modifier les propriétés de police via la référence RenderingFont
            font.Bold = true;
            
            // Afficher les propriétés de police mises à jour à partir du filigrane
            Console.WriteLine("\nUpdated Font Name: " + watermark.Font.Name);
            Console.WriteLine("Updated Font Size: " + watermark.Font.Size);
            Console.WriteLine("Updated Bold Status: " + watermark.Font.Bold);
            
            // Configurer les propriétés d'affichage du filigrane
            watermark.Opacity = 0.5f;
            watermark.Rotation = 45;
            watermark.IsBackground = true;
            
            // Créer des options d'enregistrement PDF et assigner le filigrane
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.Watermark = watermark;
            
            // Enregistrer le classeur avec le PDF filigrané pour afficher les modifications de police
            workbook.Save("RenderingWatermarkFontDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Voir aussi

* class [RenderingFont](../../renderingfont/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


