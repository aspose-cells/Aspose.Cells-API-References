---
title: "PageSetup.HeaderMarginInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Représente la distance du haut de la page à l'en-tête en pouces"
type: docs
url: /fr/net/aspose.cells/pagesetup/headermargininch/
---
## PageSetup.HeaderMarginInch property

Représente la distance entre le haut de la page et l'en-tête, en pouces.

```csharp
public double HeaderMarginInch { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyHeaderMarginInchDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accédez à la première feuille de calcul et à son PageSetup
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Définir la marge d'en-tête en pouces
            pageSetup.HeaderMarginInch = 0.5;
            
            // Définir d'autres marges à titre d'exemple
            pageSetup.FooterMarginInch = 0.25;
            pageSetup.TopMarginInch = 1.0;
            pageSetup.BottomMarginInch = 1.0;
            pageSetup.LeftMarginInch = 0.75;
            pageSetup.RightMarginInch = 0.75;

            // Enregistrez le classeur
            workbook.Save("PageSetupMargins.xlsx");

            // Afficher la valeur de la marge d'en-tête
            Console.WriteLine("Header Margin (inches): " + pageSetup.HeaderMarginInch);
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


