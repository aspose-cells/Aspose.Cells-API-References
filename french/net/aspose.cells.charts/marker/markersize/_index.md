---
title: "Marker.MarkerSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Marker. Représente la taille du marqueur en unité de points. S'applique aux graphiques en ligne, aux graphiques en nuage de points ou aux graphiques radar"
type: docs
url: /fr/net/aspose.cells.charts/marker/markersize/
---
## Marker.MarkerSize property

Représente la taille du marqueur en unité de points. S'applique aux graphiques en ligne, aux graphiques en nuage de points ou aux graphiques radar.

```csharp
public int MarkerSize { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class MarkerPropertyMarkerSizeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(i + 1);
                worksheet.Cells[i + 1, 1].PutValue((i + 1) * 2);
            }

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajouter des séries - appel de méthode corrigé
            int seriesIndex = chart.NSeries.Add("B2:B11", true);
            Series series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A11";

            // Définir les propriétés du marqueur
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.MarkerSize = 10; // Demonstrating MarkerSize property
            series.Marker.ForegroundColor = Color.Red;
            series.Marker.BackgroundColor = Color.Yellow;

            // Enregistrez le classeur
            workbook.Save("MarkerSizeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


