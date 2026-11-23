---
title: "Marker.BackgroundColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Marker. Représente la couleur d'arrière-plan du marqueur dans un graphique en courbes, un nuage de points ou un graphique radar"
type: docs
url: /fr/net/aspose.cells.charts/marker/backgroundcolor/
---
## Marker.BackgroundColor property

Représente la couleur d'arrière-plan du marqueur dans un graphique en ligne, un graphique de dispersion ou un graphique radar.

```csharp
public Color BackgroundColor { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MarkerPropertyBackgroundColorDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.LineWithDataMarkers, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Personnaliser l'apparence du marqueur
            foreach (Series series in chart.NSeries)
            {
                series.Marker.MarkerStyle = ChartMarkerType.Circle;
                series.Marker.MarkerSize = 12;
                series.Marker.Border.Color = System.Drawing.Color.Blue;
                series.Marker.BackgroundColor = System.Drawing.Color.LightGreen; // Demonstrating BackgroundColor property
            }

            workbook.Save("MarkerBackgroundColorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


