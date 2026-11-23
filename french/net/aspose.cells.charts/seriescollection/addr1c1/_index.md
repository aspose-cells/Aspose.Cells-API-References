---
title: "SeriesCollection.AddR1C1"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SeriesCollection. Ajoute la collection Series à un graphique"
type: docs
url: /fr/net/aspose.cells.charts/seriescollection/addr1c1/
---
## SeriesCollection.AddR1C1 method

Ajoute la collection [`Series`](../../series/) à un graphique.

```csharp
public int AddR1C1(string area, bool isVertical)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| zone | String | Spécifie les valeurs à partir desquelles tracer la série de données |
| isVertical | Boolean | Spécifie s'il faut tracer la série à partir d'une plage de valeurs de cellules par ligne ou par colonne. |

### Valeur de retour

Renvoie le premier indice de l'ASeries ajouté dans le NSeries.

### Remarques

Si les données sont définies sur des cellules contiguës, utilisez deux-points pour les séparer. Par exemple, R[1]C[1]:R[3]C[2]. Si les données sont définies sur des cellules contiguës, utilisez une virgule pour les séparer. Par exemple, (R[1]C[1],R[3]C[2]).

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodAddR1C1WithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet wsData = workbook.Worksheets[0];
            wsData.Name = "ChartData";

            // Données d'exemple
            wsData.Cells[0, 0].PutValue(1);
            wsData.Cells[1, 0].PutValue(2);
            wsData.Cells[0, 1].PutValue(3);
            wsData.Cells[1, 1].PutValue(4);

            Worksheet wsChart = workbook.Worksheets[workbook.Worksheets.Add(Aspose.Cells.SheetType.Chart)];
            wsChart.Name = "ChartSheet";

            int chartIndex = wsChart.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 0, 0, 15, 15);
            Aspose.Cells.Charts.Chart chart = wsChart.Charts[chartIndex];

            // Utilisation de AddR1C1 avec des paramètres String et Boolean
            int seriesIndex = chart.NSeries.AddR1C1("ChartData!R1C2:R2C2", true);
            Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];
            series.XValues = "ChartData!R1C1:R2C1";

            workbook.Save("SeriesCollectionAddR1C1Demo.xlsx", Aspose.Cells.SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


