---
title: "Interface IPageSavingCallback"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Rendering.IPageSavingCallback interface. Contrôle/Indique la progression du processus d’enregistrement des pages"
type: docs
url: /fr/net/aspose.cells.rendering/ipagesavingcallback/
---
## IPageSavingCallback interface

Contrôler/Indiquer la progression du processus d'enregistrement de la page.

```csharp
public interface IPageSavingCallback
```

## Méthodes

| Nom | Description |
| --- | --- |
| [PageEndSaving](../../aspose.cells.rendering/ipagesavingcallback/pageendsaving/)(PageEndSavingArgs) | Contrôle/Indique la fin d’une page à exporter. |
| [PageStartSaving](../../aspose.cells.rendering/ipagesavingcallback/pagestartsaving/)(PageStartSavingArgs) | Contrôle/Indique le début d’une page à exporter. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageSavingCallbackDemo : IPageSavingCallback
    {
        public static void PageSavingCallbackExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Créez des options d’enregistrement avec un rappel d’enregistrement de page
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.PageSavingCallback = new PageSavingCallbackDemo();

            // Enregistrez le classeur au format DOCX
            workbook.Save("PageSavingCallbackExample.docx", saveOptions);
        }

        // Implémentez la méthode PageStartSaving
        public void PageStartSaving(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex}");
        }

        // Implémentez la méthode PageEndSaving
        public void PageEndSaving(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex}");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


