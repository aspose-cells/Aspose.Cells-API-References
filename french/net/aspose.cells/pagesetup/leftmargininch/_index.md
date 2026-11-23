---
title: "PageSetup.LeftMarginInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Représente la taille de la marge gauche en pouces"
type: docs
url: /fr/net/aspose.cells/pagesetup/leftmargininch/
---
## PageSetup.LeftMarginInch property

Représente la taille de la marge gauche, en pouces.

```csharp
public double LeftMarginInch { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyLeftMarginInchDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Accédez à PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Définir la marge gauche en pouces (0,39 pouce = ~1 cm)
            pageSetup.LeftMarginInch = 0.39;

            // Ajoutez des données pour démontrer la marge
            worksheet.Cells["A1"].PutValue("Left Margin Demonstration");
            worksheet.Cells["A2"].PutValue("Left margin set to 0.39 inches");

            // Enregistrez le classeur
            workbook.Save("LeftMarginInchDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


