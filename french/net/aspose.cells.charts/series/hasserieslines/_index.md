---
title: "Series.HasSeriesLines"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Vrai si un graphique à colonnes empilées ou un graphique à barres possède des lignes de série ou si un graphique Pie of Pie ou Bar of Pie possède des lignes de connexion entre les deux sections. S'applique uniquement aux graphiques à colonnes empilées, graphiques à barres, graphiques Pie of Pie ou Bar of Pie"
type: docs
url: /fr/net/aspose.cells.charts/series/hasserieslines/
---
## Series.HasSeriesLines property

Vrai si un graphique à colonnes empilées ou à barres possède des lignes de séries ou si un graphique « Pie of Pie » ou « Bar of Pie » possède des lignes de connexion entre les deux sections. S'applique uniquement aux graphiques à colonnes empilées, à barres, « Pie of Pie » ou « Bar of Pie ».

```csharp
public bool HasSeriesLines { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasSeriesLinesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Q3");

            // Ajouter un graphique à colonnes empilées
            int chartIndex = worksheet.Charts.Add(ChartType.ColumnStacked, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ajouter des données de série
            chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "C1:C3";

            // Accéder à la première série
            Series series = chart.NSeries[0];
            
            // Démontrer la propriété HasSeriesLines
            series.HasSeriesLines = true; // Enable series lines
            
            // Enregistrez le classeur
            workbook.Save("SeriesHasSeriesLinesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


