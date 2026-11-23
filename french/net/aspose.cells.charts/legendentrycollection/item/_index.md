---
title: "LegendEntryCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LegendEntryCollection. Obtient l'élément LegendEntry à l'index spécifié"
type: docs
url: /fr/net/aspose.cells.charts/legendentrycollection/item/
---
## LegendEntryCollection indexer

Obtient l'élément [`LegendEntry`](../../legendentry/) à l'index spécifié.

```csharp
public LegendEntry this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice à base zéro de l'élément. |

### Valeur de retour

L’élément à l’index spécifié.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendEntryCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Category 2");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // Créer un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("A2:B3", true);
            chart.NSeries.CategoryData = "A1:B1";

            // Accéder aux entrées de légende
            LegendEntryCollection legendEntries = chart.Legend.LegendEntries;
            
            // Démontrer l'utilisation de la propriété Item
            for (int i = 0; i < legendEntries.Count; i++)
            {
                LegendEntry entry = legendEntries[i];
                Console.WriteLine($"Legend Entry {i}:");
                Console.WriteLine($"- Font: {entry.Font.Name}");
                Console.WriteLine($"- Auto Scale Font: {entry.AutoScaleFont}");
            }

            // Modifier la première entrée de légende
            if (legendEntries.Count > 0)
            {
                legendEntries[0].Font.Name = "Arial";
                legendEntries[0].Font.Size = 12;
                legendEntries[0].AutoScaleFont = false;
            }
        }
    }
}
```

### Voir aussi

* class [LegendEntry](../../legendentry/)
* class [LegendEntryCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


