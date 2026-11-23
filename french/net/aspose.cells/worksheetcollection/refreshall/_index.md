---
title: "WorksheetCollection.RefreshAll"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WorksheetCollection. Rafraîchir tous les tableaux croisés dynamiques et graphiques avec la source pivot"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/refreshall/
---
## WorksheetCollection.RefreshAll method

Rafraîchir tous les tableaux croisés dynamiques et graphiques avec la source pivot.

```csharp
[Obsolete("Use Workbook.RefreshAll() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void RefreshAll()
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode Workbook.RefreshAll(). Cette méthode sera supprimée 12 mois plus tard à compter d’avril 2026. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRefreshAllDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple et des formules
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["B3"].PutValue(1.8);
            
            // Ajouter des formules qui seront rafraîchies
            worksheet.Cells["C1"].PutValue("Total");
            worksheet.Cells["C2"].PutValue("=SUM(B2:B3)");
            
            // Modifier certaines valeurs
            worksheet.Cells["B2"].PutValue(3.0);
            worksheet.Cells["B3"].PutValue(2.0);
            
            // Rafraîchir toutes les formules dans toutes les feuilles de calcul
            workbook.Worksheets.RefreshAll();
            
            // Afficher le total rafraîchi
            Console.WriteLine("Refreshed total: " + worksheet.Cells["C2"].StringValue);
        }
    }
}
```

### Voir aussi

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


