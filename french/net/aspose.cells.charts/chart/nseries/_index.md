---
title: "Chart.NSeries"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Chart propriété. Obtient une collection SeriesCollection représentant les séries de données dans le graphique"
type: docs
url: /fr/net/aspose.cells.charts/chart/nseries/
---
## Chart.NSeries property

Obtient une collection [`SeriesCollection`](../../seriescollection/) représentant les séries de données dans le graphique.

```csharp
public SeriesCollection NSeries { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyNSeriesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple aux cellules
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Cat " + (i - 1));
                sheet.Cells["B" + i].PutValue(i * 10);
            }

            // Ajoutez un graphique
            int chartIndex = sheet.Charts.Add(ChartType.LineWithDataMarkers, 5, 2, 25, 11);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];

            // Définir la source de données pour les séries du graphique en utilisant NSeries
            chart.NSeries.Add("=Sheet1!$A$2:$B$10", true);

            // Définir le titre du graphique
            chart.Title.Text = "NSeries Demo Chart";

            // Enregistrez le classeur
            workbook.Save("NSeriesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


