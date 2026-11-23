---
title: "DataLabels.ShowSeriesName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataLabels. Indique si le nom de la série s'affiche sur les étiquettes de données d'un graphique. True pour afficher le nom de la série. False pour masquer"
type: docs
url: /fr/net/aspose.cells.charts/datalabels/showseriesname/
---
## DataLabels.ShowSeriesName property

Indique si le nom de la série s'affiche sur les étiquettes de données d'un graphique. Vrai pour afficher le nom de la série. Faux pour masquer.

```csharp
public bool ShowSeriesName { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowSeriesNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B1"].PutValue("Series 2");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Ajouter un graphique en colonnes
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries.Add("B1:B4", true);

            // Activer les étiquettes de données pour la première série
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;

            // Activer l'affichage du nom de la série pour l'étiquette de données d'un point spécifique
            var points = series.Points;
            points[1].DataLabels.ShowSeriesName = true;

            // Calculer le graphique
            chart.Calculate();

            // Enregistrez le classeur
            workbook.Save("DataLabelsShowSeriesNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


