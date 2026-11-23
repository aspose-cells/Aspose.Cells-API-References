---
title: "Chart.FilteredNSeries"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Chart. Obtient une collection SeriesCollection représentant les séries de données filtrées dans le graphique"
type: docs
url: /fr/net/aspose.cells.charts/chart/filterednseries/
---
## Chart.FilteredNSeries property

Obtient une collection [`SeriesCollection`](../../seriescollection/) représentant les séries de données filtrées dans le graphique.

```csharp
public SeriesCollection FilteredNSeries { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyFilteredNSeriesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Series");
            worksheet.Cells["A2"].PutValue("Series 1");
            worksheet.Cells["A3"].PutValue("Series 2");
            worksheet.Cells["A4"].PutValue("Series 3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique et définir certaines séries comme filtrées
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Filtrer certaines séries (masquer la Série 2)
            chart.NSeries[1].IsFiltered = true;

            // Accéder à la collection de séries filtrées
            Aspose.Cells.Charts.SeriesCollection filteredSeries = chart.FilteredNSeries;
            Console.WriteLine("Filtered Series Count: " + filteredSeries.Count.ToString());

            // Enregistrez le classeur
            workbook.Save("FilteredNSeriesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


