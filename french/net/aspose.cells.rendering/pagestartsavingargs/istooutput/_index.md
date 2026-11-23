---
title: "PageStartSavingArgs.IsToOutput"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageStartSavingArgs. Obtient ou définit une valeur indiquant si la page doit être sortie. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells.rendering/pagestartsavingargs/istooutput/
---
## PageStartSavingArgs.IsToOutput property

Obtient ou définit une valeur indiquant si la page doit être sortie. La valeur par défaut est true.

```csharp
public bool IsToOutput { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageStartSavingArgsPropertyIsToOutputDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir les données pour créer plusieurs pages
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].Value = "Data Row " + (i + 1);
                // Corrigé : Accéder à la hauteur des lignes via la collection Rows de la feuille de calcul
                worksheet.Cells.Rows[i].Height = 50;
            }

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new CustomPageSavingCallback();

            workbook.Save("PageOutputDemo.pdf", saveOptions);
        }

        private class CustomPageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                // Lire la valeur actuelle
                Console.WriteLine($"Page {args.PageIndex + 1} - Initial IsToOutput: {args.IsToOutput}");

                // Ignorer chaque page paire (numérotation à partir de 1)
                if ((args.PageIndex + 1) % 2 == 0)
                {
                    args.IsToOutput = false;
                    Console.WriteLine($"Disabling output for page {args.PageIndex + 1}");
                }
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Implémentation non requise pour cette démonstration
            }
        }
    }
}
```

### Voir aussi

* class [PageStartSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


