---
title: "PageSetup.PrintTitleColumns"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Représente les colonnes contenant les cellules à répéter sur le côté gauche de chaque page"
type: docs
url: /fr/net/aspose.cells/pagesetup/printtitlecolumns/
---
## PageSetup.PrintTitleColumns property

Représente les colonnes contenant les cellules à répéter sur le côté gauche de chaque page.

```csharp
public string PrintTitleColumns { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintTitleColumnsDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder à la configuration de la page
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Définir les colonnes de titre d'impression pour répéter la colonne A sur chaque page imprimée
            pageSetup.PrintTitleColumns = "$A:$A";
            
            // Ajouter des données à la colonne A pour démontrer l'effet
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[$"A{i + 1}"].PutValue($"Title Column - Row {i + 1}");
            }
            
            // Enregistrez le classeur
            workbook.Save("PrintTitleColumnsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


