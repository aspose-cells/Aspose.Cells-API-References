---
title: "PageSetup.PrintGridlines"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Indique si les lignes de grille des cellules sont imprimées sur la page"
type: docs
url: /fr/net/aspose.cells/pagesetup/printgridlines/
---
## PageSetup.PrintGridlines property

Indique si les lignes de grille des cellules sont imprimées sur la page.

```csharp
public bool PrintGridlines { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintGridlinesDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Placez des données d'exemple dans la cellule
            worksheet.Cells["A1"].PutValue("PrintGridlines Property Demo");
            worksheet.Cells["A3"].PutValue("Gridlines will ");
            worksheet.Cells["B3"].PutValue(worksheet.PageSetup.PrintGridlines ? "appear" : "not appear");
            worksheet.Cells["A4"].PutValue("when printing this sheet.");

            // Basculez la propriété PrintGridlines
            worksheet.PageSetup.PrintGridlines = true;
            
            // Enregistrez le classeur
            workbook.Save("PrintGridlinesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


