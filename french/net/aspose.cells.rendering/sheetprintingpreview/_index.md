---
title: "Classe SheetPrintingPreview"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Rendering.SheetPrintingPreview. Aperçu de l'impression de la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.rendering/sheetprintingpreview/
---
## SheetPrintingPreview class

Aperçu d'impression de la feuille de calcul.

```csharp
public class SheetPrintingPreview
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [SheetPrintingPreview](sheetprintingpreview/)(Worksheet, ImageOrPrintOptions) | La construction de SheetPrintingPreview |

## Propriétés

| Nom | Description |
| --- | --- |
| [EvaluatedPageCount](../../aspose.cells.rendering/sheetprintingpreview/evaluatedpagecount/) { get; } | Évaluer le nombre total de pages de cette feuille de calcul |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetPrintingPreviewDemo
    {
        public static void SheetPrintingPreviewExample()
        {
            // Charger un classeur existant
            Workbook workbook = new Workbook("SheetPrintingPreviewDemo_original.xlsx");

            // Obtenir la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une instance de ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Créer une instance de SheetPrintingPreview
            SheetPrintingPreview sheetPrintingPreview = new SheetPrintingPreview(worksheet, options);

            // Évaluer et imprimer le nombre total de pages de la feuille de calcul
            Console.WriteLine("Total Page Count: " + sheetPrintingPreview.EvaluatedPageCount);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


