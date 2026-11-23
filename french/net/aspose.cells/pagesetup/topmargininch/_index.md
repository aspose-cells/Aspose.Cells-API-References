---
title: "PageSetup.TopMarginInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Représente la taille de la marge supérieure en unités de pouces"
type: docs
url: /fr/net/aspose.cells/pagesetup/topmargininch/
---
## PageSetup.TopMarginInch property

Représente la taille de la marge supérieure, en pouces.

```csharp
public double TopMarginInch { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyTopMarginInchDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Définissez la marge supérieure à 1,5 pouces
            sheet.PageSetup.TopMarginInch = 1.5;

            // Obtenez et affichez la valeur de la marge supérieure
            Console.WriteLine("Top Margin (inches): " + sheet.PageSetup.TopMarginInch);

            // Enregistrez le classeur
            workbook.Save("PageSetup_TopMarginInch_Example.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


