---
title: "PageEndSavingArgs.HasMorePages"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageEndSavingArgs. Obtient ou définit une valeur indiquant s'il reste d'autres pages à générer. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells.rendering/pageendsavingargs/hasmorepages/
---
## PageEndSavingArgs.HasMorePages property

Obtient ou définit une valeur indiquant s’il y a plus de pages à générer. La valeur par défaut est true.

```csharp
public bool HasMorePages { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageEndSavingArgsPropertyHasMorePagesDemo
    {
        public static void Run()
        {
            // Créer un classeur avec des données s'étendant sur plusieurs pages
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[i, 0].Value = $"Row {i + 1}";
            }

            // Créer des options d'enregistrement PDF avec une gestion personnalisée des pages
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new PageControlCallback();

            // Enregistrer le classeur avec une limitation de pages
            workbook.Save("PropertyHasMorePagesDemo.pdf", saveOptions);
        }
    }

    internal class PageControlCallback : IPageSavingCallback
    {
        private int pageCount = 0;

        public void PageStartSaving(PageStartSavingArgs args)
        {
            // Non utilisé dans cette démonstration
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            // Lire la valeur actuelle de la propriété
            Console.WriteLine($"Page {pageCount} - Initial HasMorePages: {args.HasMorePages}");

            // Modifier la propriété après la première page
            if (pageCount == 0)
            {
                args.HasMorePages = false;
                Console.WriteLine($"Page {pageCount} - Updated HasMorePages: {args.HasMorePages}");
            }

            pageCount++;
        }
    }
}
```

### Voir aussi

* class [PageEndSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


