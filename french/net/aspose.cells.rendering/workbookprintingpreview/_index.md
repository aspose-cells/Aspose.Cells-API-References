---
title: "Classe WorkbookPrintingPreview"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Rendering.WorkbookPrintingPreview. Aperçu de l'impression du classeur"
type: docs
url: /fr/net/aspose.cells.rendering/workbookprintingpreview/
---
## WorkbookPrintingPreview class

Aperçu d'impression du classeur.

```csharp
public class WorkbookPrintingPreview
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [WorkbookPrintingPreview](workbookprintingpreview/)(Workbook, ImageOrPrintOptions) | La construction de WorkbookPrintingPreview |

## Propriétés

| Nom | Description |
| --- | --- |
| [EvaluatedPageCount](../../aspose.cells.rendering/workbookprintingpreview/evaluatedpagecount/) { get; } | Évaluer le nombre total de pages de ce classeur |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class WorkbookPrintingPreviewDemo
    {
        public static void WorkbookPrintingPreviewExample()
        {
            // Charger un classeur existant
            Workbook workbook = new Workbook("WorkbookPrintingPreviewExample_original.xlsx");

            // Créer une instance de ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Créer une instance de WorkbookPrintingPreview
            WorkbookPrintingPreview workbookPrintingPreview = new WorkbookPrintingPreview(workbook, options);

            // Évaluer le nombre total de pages du classeur
            int pageCount = workbookPrintingPreview.EvaluatedPageCount;

            // Imprimer le nombre de pages évalué
            Console.WriteLine("Total Page Count: " + pageCount);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


