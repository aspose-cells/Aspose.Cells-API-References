---
title: "SeriesCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SeriesCollection. Obtient l'élément Series à l'index spécifié"
type: docs
url: /fr/net/aspose.cells.charts/seriescollection/item/
---
## SeriesCollection indexer

Obtient l'élément [`Series`](../../series/) à l'index spécifié.

```csharp
public Series this[int index] { get; }
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
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Series");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["B1"].PutValue("Values");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accédez à la première série et à son premier point en utilisant la propriété Item
            Series series = chart.NSeries[0];
            ChartPoint point = series.Points[0];

            // Personnaliser l'apparence du point
            point.Area.FillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.White, GradientStyleType.Vertical, 2);
            point.Area.FillFormat.FillType = FillType.Solid;

            // Enregistrez le classeur
            workbook.Save("SeriesCollectionPropertyItemDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [Series](../../series/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


