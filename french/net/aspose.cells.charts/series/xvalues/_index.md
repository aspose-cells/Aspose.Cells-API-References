---
title: "Series.XValues"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Représente les valeurs X de cette série de graphique"
type: docs
url: /fr/net/aspose.cells.charts/series/xvalues/
---
## Series.XValues property

Représente les valeurs X de cette série de graphique.

```csharp
public string XValues { get; set; }
```

### Remarques

Uniquement pour les graphiques en nuage de points et à bulles. Veuillez utiliser [`CategoryData`](../../seriescollection/categorydata/) pour les autres types de graphiques. [`CategoryValues`](../categoryvalues/) est utilisé pour obtenir les valeurs de catégorie réelles de cette série.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyXValuesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            var workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["C1"].PutValue("Series 2");
            
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i+1, 0].PutValue(i+1); // X values 1-5
                worksheet.Cells[i+1, 1].PutValue((i+1)*2); // Series 1 values
                worksheet.Cells[i+1, 2].PutValue((i+1)*3); // Series 2 values
            }

            // Ajouter un graphique en nuage de points
            int chartIndex = worksheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajouter une série avec XValues et Values
            int seriesIndex = chart.NSeries.Add("B2:B6", false);
            Series series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A6"; // Demonstrating XValues property
            series.Name = "Series 1";

            seriesIndex = chart.NSeries.Add("C2:C6", false);
            series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A6"; // Demonstrating XValues property again
            series.Name = "Series 2";

            // Enregistrez le classeur
            workbook.Save("SeriesXValuesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


