---
title: "PivotTable.RefreshedByWho"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Obtient le nom du dernier utilisateur qui a actualisé ce PivotTable"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/refreshedbywho/
---
## PivotTable.RefreshedByWho property

Obtient le nom du dernier utilisateur qui a actualisé ce PivotTable

```csharp
public string RefreshedByWho { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRefreshedByWhoDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 8;

            // Créer un tableau croisé dynamique
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pt = sheet.PivotTables[pivotIndex];
            
            // Ajouter des champs au tableau croisé dynamique
            pt.AddFieldToArea(PivotFieldType.Row, 0);
            pt.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Actualiser le tableau croisé dynamique pour définir la propriété RefreshedByWho
            pt.RefreshData();
            pt.CalculateData();

            // Afficher les informations d’actualisation
            Console.WriteLine("Pivot Table Refresh Information:");
            Console.WriteLine("Last Refresh Date: " + pt.RefreshDate);
            Console.WriteLine("Refreshed By: " + pt.RefreshedByWho);
            
            // Enregistrer et recharger pour démontrer la persistance de la propriété
            string savePath = "PivotTableRefreshedByWhoDemo_Out.xlsx";
            wb.Save(savePath);
            
            // Recharger le classeur et vérifier la propriété
            Workbook wb2 = new Workbook(savePath);
            PivotTable pt2 = wb2.Worksheets[0].PivotTables[0];
            Console.WriteLine("\nAfter Reload:");
            Console.WriteLine("Last Refresh Date: " + pt2.RefreshDate);
            Console.WriteLine("Refreshed By: " + pt2.RefreshedByWho);
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


