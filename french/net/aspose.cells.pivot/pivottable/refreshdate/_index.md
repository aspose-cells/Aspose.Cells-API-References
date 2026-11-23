---
title: "PivotTable.RefreshDate"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "PivotTable property. Obtient la dernière date et heure à laquelle le tableau croisé dynamique a été actualisé"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/refreshdate/
---
## PivotTable.RefreshDate property

Obtient la dernière date et heure à laquelle le PivotTable a été actualisé.

```csharp
public DateTime RefreshDate { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRefreshDateDemo
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

            // Ajouter un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pt = sheet.PivotTables[index];
            
            // Actualisez le tableau croisé dynamique pour définir la date d’actualisation
            pt.RefreshData();
            pt.CalculateData();

            // Affichez les informations de date d’actualisation
            Console.WriteLine("Pivot Table Refresh Date: " + pt.RefreshDate.ToLongDateString());
            Console.WriteLine("Refreshed By: " + pt.RefreshedByWho);

            // Enregistrer et recharger pour démontrer la persistance
            string savePath = "PivotTableRefreshDateDemo_Out.xlsx";
            wb.Save(savePath);
            
            // Rechargez et affichez à nouveau la date d’actualisation
            Workbook wb2 = new Workbook(savePath);
            PivotTable pt2 = wb2.Worksheets[0].PivotTables[0];
            Console.WriteLine("\nAfter reloading:");
            Console.WriteLine("Pivot Table Refresh Date: " + pt2.RefreshDate.ToLongDateString());
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


