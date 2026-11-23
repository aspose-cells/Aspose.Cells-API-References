---
title: "Classe PageSavingArgs"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Rendering.PageSavingArgs. Informations sur le processus d'enregistrement d'une page"
type: docs
url: /fr/net/aspose.cells.rendering/pagesavingargs/
---
## PageSavingArgs class

Informations pour le processus d'enregistrement d'une page.

```csharp
public class PageSavingArgs
```

## Propriétés

| Nom | Description |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Nombre total de pages. |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Index de la page actuelle, basé sur zéro. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassPageSavingArgsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec des données étendues pour plusieurs pages
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplir la feuille de calcul pour générer plusieurs pages lors du rendu
            for (int row = 0; row < 150; row++)
            {
                worksheet.Cells[row, 0].Value = $"Row {row + 1} data";
            }

            // Configurer les options d'enregistrement PDF avec le rappel d'enregistrement de page
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.PageSavingCallback = new PageSavingCallback();

            // Enregistrer le classeur au format PDF avec pagination
            workbook.Save("RenderingPageSavingDemo.pdf", pdfSaveOptions);
        }

        private class PageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                Console.WriteLine($"Saving page {args.PageIndex + 1} of {args.PageCount}");
                
                if (args.PageIndex == 0)
                {
                    Console.WriteLine("Processing cover page...");
                }
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Optionnel : ajoutez tout traitement de fin de page ici
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


