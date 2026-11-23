---
title: "IPageSavingCallback.PageStartSaving"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode IPageSavingCallback. Contrôler/Indiquer le début d'une page à sortir"
type: docs
url: /fr/net/aspose.cells.rendering/ipagesavingcallback/pagestartsaving/
---
## IPageSavingCallback.PageStartSaving method

Contrôle/Indique le début d’une page à exporter.

```csharp
public void PageStartSaving(PageStartSavingArgs args)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| args | PageStartSavingArgs | Informations pour le processus de démarrage de l'enregistrement d'une page. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class IPageSavingCallbackMethodPageStartSavingWithPageStartSavingArgsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter du contenu d'exemple pour créer plusieurs pages
            for (int i = 0; i < 150; i++)
                worksheet.Cells[$"A{i + 1}"].Value = $"Data row {i + 1}";

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            PageSavingCallback callback = new PageSavingCallback();
            saveOptions.PageSavingCallback = callback;

            try
            {
                workbook.Save("PageStartSavingOutput.pdf", saveOptions);
                Console.WriteLine($"Processed pages: {callback.ProcessedPages}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class PageSavingCallback : IPageSavingCallback
    {
        public int ProcessedPages { get; private set; }

        public void PageStartSaving(PageStartSavingArgs args)
        {
            if (args.PageIndex % 3 == 0) // Skip every 3rd page (0-based)
                args.IsToOutput = false;
            else
                ProcessedPages++;

            Console.WriteLine(args.IsToOutput 
                ? $"Saving page {args.PageIndex + 1}"
                : $"Skipping page {args.PageIndex + 1}");
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            // Gestion optionnelle de la fin de page
        }
    }
}
```

### Voir aussi

* class [PageStartSavingArgs](../../pagestartsavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


