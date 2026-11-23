---
title: "IPageSavingCallback.PageEndSaving"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode IPageSavingCallback. Contrôler/Indiquer la fin d'une page à sortir"
type: docs
url: /fr/net/aspose.cells.rendering/ipagesavingcallback/pageendsaving/
---
## IPageSavingCallback.PageEndSaving method

Contrôle/Indique la fin d’une page à exporter.

```csharp
public void PageEndSaving(PageEndSavingArgs args)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| args | PageEndSavingArgs | Les informations d'une page terminent le processus d'enregistrement. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class IPageSavingCallbackMethodPageEndSavingWithPageEndSavingArgsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et remplir les données
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour créer plusieurs pages lors du rendu
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[$"A{i+1}"].Value = $"Row {i+1} - Demonstration data for page splitting";
            }

            // Créer des options d'enregistrement PDF avec un rappel de sauvegarde de page personnalisé
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new PageEndSavingCallback();

            try
            {
                // Enregistrer le classeur avec l'implémentation du rappel
                workbook.Save("PageEndSavingDemo.pdf", saveOptions);
                Console.WriteLine("Document saved successfully with page end tracking.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during document save: {ex.Message}");
            }
        }

        private class PageEndSavingCallback : IPageSavingCallback
        {
            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Afficher les informations de fin de sauvegarde de page
                Console.WriteLine($"Finished processing page {args.PageIndex + 1}");
                
                // Vous pouvez ajouter des opérations de fichier ou d'autres post-traitements ici
                // args.HasMorePages indique si d'autres pages seront traitées
            }

            public void PageStartSaving(PageStartSavingArgs args)
            {
                // Implémentation d'interface requise
            }
        }
    }
}
```

### Voir aussi

* class [PageEndSavingArgs](../../pageendsavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


