---
title: "PageSetup.BottomMarginInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Représente la taille de la marge inférieure en pouces"
type: docs
url: /fr/net/aspose.cells/pagesetup/bottommargininch/
---
## PageSetup.BottomMarginInch property

Indique la taille de la marge inférieure, en pouces.

```csharp
public double BottomMarginInch { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyBottomMarginInchDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accédez au PageSetup de la première feuille de calcul
            PageSetup setup = workbook.Worksheets[0].PageSetup;
            
            // Définir diverses marges en pouces
            setup.HeaderMarginInch = 0.1;
            setup.FooterMarginInch = 0.2;
            setup.TopMarginInch = 0.3;
            setup.BottomMarginInch = 0.4; // Demonstrating BottomMarginInch property
            setup.LeftMarginInch = 0.5;
            setup.RightMarginInch = 0.6;
            
            // Enregistrez le classeur
            workbook.Save("PageMarginsDemo.xlsx");
            
            // Afficher la confirmation
            Console.WriteLine("Workbook saved with bottom margin set to: " + setup.BottomMarginInch + " inches");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


