---
title: "SheetPrintingPreview.SheetPrintingPreview"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur SheetPrintingPreview. La construction de SheetPrintingPreview"
type: docs
url: /fr/net/aspose.cells.rendering/sheetprintingpreview/sheetprintingpreview/
---
## SheetPrintingPreview constructor

La construction de SheetPrintingPreview

```csharp
public SheetPrintingPreview(Worksheet sheet, ImageOrPrintOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| feuille | Feuille de calcul | Indiquer quelle feuille de calcul doit être imprimée. |
| options | ImageOrPrintOptions | ImageOrPrintOptions contient certaines propriétés de sortie |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetPrintingPreviewMethodctorWithWorksheetImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple à la feuille de calcul
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Créer des options d'image/impression
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.Default;

            // Créer un aperçu d’impression de feuille
            SheetPrintingPreview preview = new SheetPrintingPreview(worksheet, options);
            
            // Afficher le nombre de pages évalué
            Console.WriteLine($"Evaluated page count: {preview.EvaluatedPageCount}");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


