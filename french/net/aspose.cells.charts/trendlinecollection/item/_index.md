---
title: "TrendlineCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TrendlineCollection. Obtient un objet Trendline par son indice"
type: docs
url: /fr/net/aspose.cells.charts/trendlinecollection/item/
---
## TrendlineCollection indexer

Obtient un objet [`Trendline`](../../trendline/) par son indice.

```csharp
public Trendline this[int index] { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlineCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue(1);
            sheet.Cells["A2"].PutValue(2);
            sheet.Cells["A3"].PutValue(3);
            sheet.Cells["B1"].PutValue(4);
            sheet.Cells["B2"].PutValue(5);
            sheet.Cells["B3"].PutValue(6);

            // Ajoutez un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries[0].Values = "B1:B3";

            // Ajouter une Trendline
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];

            // Démontrer l'utilisation de la propriété Item
            Trendline firstTrendline = chart.NSeries[0].TrendLines[0];
            Console.WriteLine("Trendline Type: " + firstTrendline.Type);
        }
    }
}
```

### Voir aussi

* class [Trendline](../../trendline/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


