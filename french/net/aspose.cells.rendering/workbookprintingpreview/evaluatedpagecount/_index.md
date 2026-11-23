---
title: "WorkbookPrintingPreview.EvaluatedPageCount"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "WorkbookPrintingPreview propriété. Évaluez le nombre total de pages de ce classeur"
type: docs
url: /fr/net/aspose.cells.rendering/workbookprintingpreview/evaluatedpagecount/
---
## WorkbookPrintingPreview.EvaluatedPageCount property

Évaluer le nombre total de pages de ce classeur

```csharp
public int EvaluatedPageCount { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookPrintingPreviewPropertyEvaluatedPageCountDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple à la feuille de calcul
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].PutValue("Row " + (i + 1));
            }

            // Créer des options d'aperçu d'impression
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Créer l'aperçu d'impression du classeur
            WorkbookPrintingPreview printingPreview = new WorkbookPrintingPreview(workbook, options);
            
            // Obtenir et afficher le nombre de pages évalué
            Console.WriteLine("Evaluated Page Count: " + printingPreview.EvaluatedPageCount);
        }
    }
}
```

### Voir aussi

* class [WorkbookPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


