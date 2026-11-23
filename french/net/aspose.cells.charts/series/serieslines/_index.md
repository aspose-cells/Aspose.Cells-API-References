---
title: "Series.SeriesLines"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Retourne un objet SeriesLines qui représente les lignes de série pour un graphique à barres empilées ou à colonnes empilées. S'applique uniquement aux graphiques à barres empilées et à colonnes empilées"
type: docs
url: /fr/net/aspose.cells.charts/series/serieslines/
---
## Series.SeriesLines property

Renvoie un objet SeriesLines qui représente les lignes de série pour un graphique à barres empilées ou un graphique à colonnes empilées. S'applique uniquement aux graphiques à barres empilées et à colonnes empilées.

```csharp
public Line SeriesLines { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertySeriesLinesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["A5"].PutValue(4);
            
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Créer un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ajouter une série
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // Personnaliser les lignes de série
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.SeriesLines.Color = Color.Red;
            series.SeriesLines.Weight = Aspose.Cells.Drawing.WeightType.SingleLine;
            
            // Enregistrez le classeur
            workbook.Save("SeriesLinesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


