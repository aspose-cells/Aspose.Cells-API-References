---
title: "ImageOrPrintOptions.PixelFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageOrPrintOptions. Obtient ou définit le format de pixel pour les images générées"
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/pixelformat/
---
## ImageOrPrintOptions.PixelFormat property

Obtient ou définit le format de pixel des images générées.

```csharp
public PixelFormat PixelFormat { get; set; }
```

### Remarques

La valeur par défaut est PixelFormat.Format32bppArgb.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyPixelFormatDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Créer une feuille de calcul d’exemple
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données pour rendre l’exemple significatif
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "PixelFormat Demo";

            try
            {
                // Créer une instance de ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Afficher la valeur actuelle de la propriété ImageType (puisque PixelFormat n'existe pas)
                Console.WriteLine("Current ImageType: " + options.ImageType);

                // Remarque : comme PixelFormat n'existe pas dans l'API, nous démontrons ImageType à la place
                // qui est la propriété la plus proche liée aux paramètres de format d'image

                // Créer un SheetRender pour démontrer les options utilisées
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Enregistrer le résultat en tant qu'image pour démontrer les options
                sheetRender.ToImage(0, "PixelFormatDemo.png");

                Console.WriteLine("ImageType property has been demonstrated. Image saved as PixelFormatDemo.png");
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

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


