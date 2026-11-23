---
title: "PageSavingArgs.PageIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSavingArgs. Index de la page actuelle basé sur zéro"
type: docs
url: /fr/net/aspose.cells.rendering/pagesavingargs/pageindex/
---
## PageSavingArgs.PageIndex property

Index de la page actuelle, basé sur zéro.

```csharp
public int PageIndex { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSavingArgsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données à la feuille de calcul
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
            }

            // Créez les options d'enregistrement PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Définir le rappel d'enregistrement de page
            options.PageSavingCallback = new PageSavingCallback();

            // Enregistrer le classeur en PDF - cela déclenchera le rappel pour chaque page
            workbook.Save("output.pdf", options);
        }
    }

    public class PageSavingCallback : IPageSavingCallback
    {
        public void PageStartSaving(PageStartSavingArgs args)
        {
            // Démontrer l'utilisation de la propriété PageIndex
            Console.WriteLine($"Starting to save page {args.PageIndex + 1}");
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            // Non utilisé dans cet exemple
        }
    }
}
```

### Voir aussi

* class [PageSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


