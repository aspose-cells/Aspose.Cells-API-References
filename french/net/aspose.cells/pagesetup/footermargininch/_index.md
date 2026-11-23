---
title: "PageSetup.FooterMarginInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Représente la distance du bas de la page au pied de page en pouces"
type: docs
url: /fr/net/aspose.cells/pagesetup/footermargininch/
---
## PageSetup.FooterMarginInch property

Représente la distance entre le bas de la page et le pied de page, en pouces.

```csharp
public double FooterMarginInch { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFooterMarginInchDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul et à son PageSetup
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Définir la marge du pied de page en pouces
            pageSetup.FooterMarginInch = 0.5;
            
            // Définir d'autres marges à titre d'exemple
            pageSetup.HeaderMarginInch = 0.3;
            pageSetup.TopMarginInch = 1.0;
            pageSetup.BottomMarginInch = 1.0;
            pageSetup.LeftMarginInch = 0.75;
            pageSetup.RightMarginInch = 0.75;
            
            // Enregistrez le classeur
            workbook.Save("PageSetupMargins.xlsx");
            
            // Imprimer la confirmation
            Console.WriteLine("Footer margin set to: " + pageSetup.FooterMarginInch + " inches");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


