---
title: "Classe PageStartSavingArgs"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Rendering.PageStartSavingArgs. Informations pour le démarrage du processus d’enregistrement d’une page"
type: docs
url: /fr/net/aspose.cells.rendering/pagestartsavingargs/
---
## PageStartSavingArgs class

Informations pour le processus de démarrage de l'enregistrement d'une page.

```csharp
public class PageStartSavingArgs : PageSavingArgs
```

## Propriétés

| Nom | Description |
| --- | --- |
| [IsToOutput](../../aspose.cells.rendering/pagestartsavingargs/istooutput/) { get; set; } | Obtient ou définit une valeur indiquant si la page doit être sortie. La valeur par défaut est true. |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Nombre total de pages.(Hérité de [`PageSavingArgs`](../pagesavingargs/).) |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Indice de page actuel, basé à zéro.(Hérité de [`PageSavingArgs`](../pagesavingargs/).) |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassPageStartSavingArgsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Hello World");
            
            PdfSaveOptions options = new PdfSaveOptions();
            options.PageSavingCallback = new CustomPageSavingCallback();
            
            workbook.Save("output.pdf", options);
        }
    }
    
    public class CustomPageSavingCallback : IPageSavingCallback
    {
        public void PageStartSaving(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex}");
        }
        
        public void PageEndSaving(PageEndSavingArgs args)
        {
            // Implémentation facultative
        }
    }
}
```

### Voir aussi

* class [PageSavingArgs](../pagesavingargs/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


