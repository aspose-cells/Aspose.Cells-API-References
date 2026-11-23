---
title: "Series.Points"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Obtient la collection de points d’une série dans un graphique"
type: docs
url: /fr/net/aspose.cells.charts/series/points/
---
## Series.Points property

Obtient la collection de points d'une série dans un graphique.

```csharp
public ChartPointCollection Points { get; }
```

### Remarques

Lorsque le graphique est un diagramme en secteurs imbriqués (Pie of Pie) ou un diagramme en barres imbriquées (Bar of Pie), le dernier point est le point « autre » du premier diagramme circulaire.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyPointsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accédez à la première série et à ses points
            Series series = chart.NSeries[0];
            foreach (ChartPoint point in series.Points)
            {
                // Ajoutez des étiquettes de données à chaque point
                point.DataLabels.ShowValue = true;
                point.DataLabels.ShowCellRange = true;
            }

            // Enregistrez le classeur
            workbook.Save("SeriesPropertyPointsDemo_Output.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPointCollection](../../chartpointcollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


