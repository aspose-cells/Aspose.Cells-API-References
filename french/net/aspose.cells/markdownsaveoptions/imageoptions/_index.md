---
title: "MarkdownSaveOptions.ImageOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MarkdownSaveOptions. Obtenez l'objet ImageOrPrintOptions avant l'exportation"
type: docs
url: /fr/net/aspose.cells/markdownsaveoptions/imageoptions/
---
## MarkdownSaveOptions.ImageOptions property

Obtenez l’objet ImageOrPrintOptions avant l’exportation

```csharp
public ImageOrPrintOptions ImageOptions { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class MarkdownSaveOptionsPropertyImageOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Créer une feuille de calcul d’exemple
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données pour rendre l’exemple significatif
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "Image Options Demo";

            try
            {
                // Créer une instance de MarkdownSaveOptions
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Accéder à la propriété ImageOptions (lecture seule)
                ImageOrPrintOptions imageOptions = saveOptions.ImageOptions;

                // Afficher les valeurs actuelles des propriétés ImageOptions
                Console.WriteLine("ImageOptions properties:");
                Console.WriteLine($"HorizontalResolution: {imageOptions.HorizontalResolution}");
                Console.WriteLine($"VerticalResolution: {imageOptions.VerticalResolution}");
                Console.WriteLine($"ImageType: {imageOptions.ImageType}");
                Console.WriteLine($"Quality: {imageOptions.Quality}");
                Console.WriteLine($"Transparent: {imageOptions.Transparent}");

                // Enregistrer le classeur avec les options actuelles
                workbook.Save("ImageOptionsDemo.md", saveOptions);

                Console.WriteLine("Markdown file saved successfully with ImageOptions demonstrated.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


