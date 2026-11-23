---
title: "PaginatedSaveOptions.PageSavingCallback"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PaginatedSaveOptions. Contrôle/Indique la progression du processus d'enregistrement des pages"
type: docs
url: /fr/net/aspose.cells/paginatedsaveoptions/pagesavingcallback/
---
## PaginatedSaveOptions.PageSavingCallback property

Contrôler/Indiquer la progression du processus d'enregistrement de la page.

```csharp
public IPageSavingCallback PageSavingCallback { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageSavingCallbackDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Page 1 Content");
            worksheet.Cells["A2"].PutValue("This demonstrates PageSavingCallback");

            // Créez des options d'enregistrement avec un rappel d'enregistrement de page
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new CustomPageSavingCallback();

            // Enregistrez avec le rappel
            workbook.Save("PageSavingCallbackDemo.pdf", saveOptions);
        }
    }

    public class CustomPageSavingCallback : IPageSavingCallback
    {
        public void PageStartSaving(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex + 1}");
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex + 1}");
            if (args.HasMorePages)
            {
                Console.WriteLine("More pages to follow...");
            }
        }
    }
}
```

### Voir aussi

* interface [IPageSavingCallback](../../../aspose.cells.rendering/ipagesavingcallback/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


