---
title: "LegendEntry.IsDeleted"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LegendEntry. Obtient et définit si l'entrée de légende est supprimée"
type: docs
url: /fr/net/aspose.cells.charts/legendentry/isdeleted/
---
## LegendEntry.IsDeleted property

Obtient et définit si l'entrée de légende est supprimée.

```csharp
public bool IsDeleted { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Obtenir la première entrée de légende
            LegendEntry legendEntry = chart.Legend.LegendEntries[0];

            // Démontrer la propriété IsDeleted
            Console.WriteLine("Legend entry initially deleted? " + legendEntry.IsDeleted);
            
            // Supprimer l'entrée de légende
            legendEntry.IsDeleted = true;
            Console.WriteLine("Legend entry after deletion? " + legendEntry.IsDeleted);

            // Restaurer l'entrée de légende
            legendEntry.IsDeleted = false;
            Console.WriteLine("Legend entry after restoration? " + legendEntry.IsDeleted);

            // Enregistrez le classeur
            workbook.Save("LegendEntryIsDeletedDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


