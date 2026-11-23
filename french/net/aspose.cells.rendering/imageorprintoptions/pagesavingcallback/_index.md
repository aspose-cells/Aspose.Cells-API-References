---
title: "ImageOrPrintOptions.PageSavingCallback"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageOrPrintOptions. Contrôler/Indiquer la progression du processus d'enregistrement des pages"
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/pagesavingcallback/
---
## ImageOrPrintOptions.PageSavingCallback property

Contrôler/Indiquer la progression du processus d'enregistrement de la page.

```csharp
public IPageSavingCallback PageSavingCallback { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyPageSavingCallbackDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et remplir les données
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple s'étendant sur plusieurs pages
            worksheet.Cells["A1"].PutValue("PageSavingCallback Demonstration");
            for (int i = 1; i <= 50; i++)
            {
                worksheet.Cells[$"A{i + 1}"].PutValue($"Data Row {i}");
            }

            // Configurer la mise en page pour générer plusieurs pages
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.PaperSize = PaperSizeType.PaperA4;
            pageSetup.Orientation = PageOrientationType.Portrait;
            pageSetup.FitToPagesWide = 1;
            pageSetup.FitToPagesTall = 0;

            // Initialiser ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT4
            };

            // Afficher l'état initial du callback
            Console.WriteLine($"Initial PageSavingCallback: {options.PageSavingCallback}");

            // Définir le callback personnalisé d'enregistrement de page
            options.PageSavingCallback = new CustomPageSavingCallback();

            // Rendre la feuille de calcul en TIFF multipage
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToTiff("output_with_callback.tiff");

            // Enregistrer le classeur pour référence
            workbook.Save("PageSavingCallbackDemo.xlsx");
        }

        private class CustomPageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                Console.WriteLine($"Processing page {args.PageIndex}");
                
                // Ignorer la première page (index basé sur 0)
                if (args.PageIndex == 0)
                {
                    args.IsToOutput = false;
                    Console.WriteLine("Skipping first page");
                }
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                Console.WriteLine($"Completed processing page {args.PageIndex}");
            }
        }
    }
}
```

### Voir aussi

* interface [IPageSavingCallback](../../ipagesavingcallback/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


