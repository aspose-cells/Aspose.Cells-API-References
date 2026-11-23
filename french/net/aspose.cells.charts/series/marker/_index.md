---
title: "Series.Marker"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété de la série. Obtient le marqueur"
type: docs
url: /fr/net/aspose.cells.charts/series/marker/
---
## Series.Marker property

Obtient le `marker`.

```csharp
public Marker Marker { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyMarkerDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);

            // Créer un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.LineWithDataMarkers, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Personnaliser les propriétés du marqueur
            foreach (Series series in chart.NSeries)
            {
                series.Marker.MarkerStyle = ChartMarkerType.SquarePlus;
                series.Marker.MarkerSize = 12;
                series.Marker.Border.Color = Color.Red;
                series.Marker.BackgroundColor = Color.Yellow;
            }

            workbook.Save("SeriesMarkerDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Marker](../../marker/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


