---
title: "PageSetup.FitToPagesWide"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Représente le nombre de pages en largeur auquel la feuille de calcul sera mise à l'échelle lors de l'impression. La valeur par défaut est 1"
type: docs
url: /fr/net/aspose.cells/pagesetup/fittopageswide/
---
## PageSetup.FitToPagesWide property

Représente le nombre de pages en largeur auquel la feuille de calcul sera mise à l'échelle lors de l'impression. La valeur par défaut est 1.

```csharp
public int FitToPagesWide { get; set; }
```

### Remarques

Vous devez définir FitToPagesTall à zéro si vous voulez ajuster toutes les colonnes sur une page.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFitToPagesWideDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Sample Data 1");
            worksheet.Cells["A2"].PutValue("Sample Data 2");
            worksheet.Cells["B1"].PutValue("Sample Data 3");
            worksheet.Cells["B2"].PutValue("Sample Data 4");

            // Définir les propriétés de mise en page
            worksheet.PageSetup.FitToPagesWide = 1;  // Fit to 1 page wide
            worksheet.PageSetup.FitToPagesTall = 0; // Let height adjust automatically

            // Enregistrez le classeur
            workbook.Save("FitToPagesWideDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


