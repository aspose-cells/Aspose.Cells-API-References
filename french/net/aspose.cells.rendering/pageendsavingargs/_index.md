---
title: "Classe PageEndSavingArgs"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Rendering.PageEndSavingArgs. Informations sur le processus de fin d’enregistrement d’une page"
type: docs
url: /fr/net/aspose.cells.rendering/pageendsavingargs/
---
## PageEndSavingArgs class

Les informations d'une page terminent le processus d'enregistrement.

```csharp
public class PageEndSavingArgs : PageSavingArgs
```

## Propriétés

| Nom | Description |
| --- | --- |
| [HasMorePages](../../aspose.cells.rendering/pageendsavingargs/hasmorepages/) { get; set; } | Obtient ou définit une valeur indiquant s’il y a plus de pages à générer. La valeur par défaut est true. |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Nombre total de pages.(Hérité de [`PageSavingArgs`](../pagesavingargs/).) |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Indice de page actuel, basé à zéro.(Hérité de [`PageSavingArgs`](../pagesavingargs/).) |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassPageEndSavingArgsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Créer une instance de PdfSaveOptions
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Définir le rappel PageEndSaving
            saveOptions.PageSavingCallback = new PageEndSavingArgsTest();

            // Enregistrer le classeur avec le rappel
            workbook.Save("output.pdf", saveOptions);
        }
    }

    public class PageEndSavingArgsTest : IPageSavingCallback
    {
        public void PageEndSaving(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex}");
        }

        public void PageStartSaving(PageStartSavingArgs args)
        {
            // Implémentation non requise pour cette démo
        }
    }
}
```

### Voir aussi

* class [PageSavingArgs](../pagesavingargs/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


