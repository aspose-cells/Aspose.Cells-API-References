---
title: "Marker.MarkerStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Marker. Représente le style du marqueur. S'applique à un graphique en ligne, à un graphique en nuage de points ou à un graphique radar"
type: docs
url: /fr/net/aspose.cells.charts/marker/markerstyle/
---
## Marker.MarkerStyle property

Représente le style du marqueur. S'applique à un graphique en ligne, un graphique en nuage de points ou un graphique radar.

```csharp
public ChartMarkerType MarkerStyle { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MarkerPropertyMarkerStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["B2"].PutValue(4);
            sheet.Cells["B3"].PutValue(5);
            sheet.Cells["B4"].PutValue(6);

            // Ajoutez un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "B2:B4";

            // Définir le style du marqueur pour la première série
            chart.NSeries[0].Marker.MarkerStyle = ChartMarkerType.Circle;
            chart.NSeries[0].Marker.ForegroundColor = System.Drawing.Color.Blue;
            chart.NSeries[0].Marker.BackgroundColor = System.Drawing.Color.White;
            chart.NSeries[0].Marker.MarkerSize = 10;

            // Enregistrez le classeur
            workbook.Save("MarkerStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ChartMarkerType](../../chartmarkertype/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


