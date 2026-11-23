---
title: "SheetRender.PageCount"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SheetRender. Obtient le nombre total de pages de la feuille de calcul actuelle"
type: docs
url: /fr/net/aspose.cells.rendering/sheetrender/pagecount/
---
## SheetRender.PageCount property

Obtient le nombre total de pages de la feuille de calcul actuelle.

```csharp
public int PageCount { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderPropertyPageCountDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Mary");
            cells["B3"].PutValue(25);
            cells["A4"].PutValue("Peter");
            cells["B4"].PutValue(35);

            // Définir la configuration de page pour l'impression
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.PrintArea = "A1:B4";
            pageSetup.FitToPagesTall = 1;
            pageSetup.FitToPagesWide = 1;

            // Créer SheetRender avec les options par défaut
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            SheetRender render = new SheetRender(worksheet, options);

            // Afficher le nombre de pages
            Console.WriteLine("Page Count: " + render.PageCount);

            // Modifier la configuration de page pour forcer plusieurs pages
            pageSetup.FitToPagesTall = 0;
            pageSetup.FitToPagesWide = 1;
            pageSetup.PrintArea = "A1:B100"; // Larger area than can fit on one page

            // Créer un nouveau SheetRender pour obtenir le nombre de pages mis à jour
            SheetRender newRender = new SheetRender(worksheet, options);
            Console.WriteLine("Updated Page Count: " + newRender.PageCount);
        }
    }
}
```

### Voir aussi

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


