---
title: "PageSetup.PrintTitleRows"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Représente les lignes contenant les cellules à répéter en haut de chaque page"
type: docs
url: /fr/net/aspose.cells/pagesetup/printtitlerows/
---
## PageSetup.PrintTitleRows property

Représente les lignes contenant les cellules à répéter en haut de chaque page.

```csharp
public string PrintTitleRows { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintTitleRowsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir des données d'exemple
            worksheet.Cells["A1"].PutValue("Header");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Data " + (i-1));
            }
            
            // Accéder à la configuration de la page
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Définir les lignes de titre d'impression (la première ligne sera répétée sur chaque page imprimée)
            pageSetup.PrintTitleRows = "$1:$1";
            
            // Enregistrez le classeur
            workbook.Save("PrintTitleRowsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


