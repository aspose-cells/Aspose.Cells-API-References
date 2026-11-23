---
title: "PageSetup.RightMarginInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Représente la taille de la marge droite en unités de pouces"
type: docs
url: /fr/net/aspose.cells/pagesetup/rightmargininch/
---
## PageSetup.RightMarginInch property

Représente la taille de la marge droite, en pouces.

```csharp
public double RightMarginInch { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyRightMarginInchDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Accédez à PageSetup et définissez RightMarginInch
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.RightMarginInch = 0.75; // Set right margin to 0.75 inches

            // Ajoutez des données d'exemple pour voir l'effet
            worksheet.Cells["A1"].PutValue("Right Margin Demo");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["B" + i].PutValue("Sample Data " + i);
            }

            // Enregistrez le classeur
            workbook.Save("RightMarginInchDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


