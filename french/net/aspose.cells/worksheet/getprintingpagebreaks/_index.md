---
title: "Worksheet.GetPrintingPageBreaks"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Obtient les sauts de page automatiques"
type: docs
url: /fr/net/aspose.cells/worksheet/getprintingpagebreaks/
---
## Worksheet.GetPrintingPageBreaks method

Obtient les sauts de page automatiques.

```csharp
public CellArea[] GetPrintingPageBreaks(ImageOrPrintOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | ImageOrPrintOptions | Les options d'impression |

### Valeur de retour

Les zones de sauts de page automatiques.

### Remarques

Chaque zone de cellule représente une feuille.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetPrintingPageBreaksWithImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple pour créer des sauts de page
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[$"A{i+1}"].PutValue($"Row {i+1}");
            }

            // Définissez la zone d'impression et la configuration de la page
            worksheet.PageSetup.PrintArea = "A1:A100";
            worksheet.PageSetup.FitToPagesTall = 1;
            worksheet.PageSetup.FitToPagesWide = 1;

            // Obtenez les sauts de page avec ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            CellArea[] pageBreaks = worksheet.GetPrintingPageBreaks(options);

            // Affichez les informations du premier saut de page
            Console.WriteLine($"First page break ends at row: {pageBreaks[0].EndRow}");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


