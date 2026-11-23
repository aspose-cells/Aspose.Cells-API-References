---
title: "Class Marker"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.Marker class. Représente le marqueur dans un graphique en ligne, un graphique de dispersion ou un graphique radar"
type: docs
url: /fr/net/aspose.cells.charts/marker/
---
## Marker class

Représente le marqueur dans un graphique en ligne, un nuage de points ou un graphique radar.

```csharp
public class Marker
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Area](../../aspose.cells.charts/marker/area/) { get; } | Obtient le [`area`](./area/). |
| [BackgroundColor](../../aspose.cells.charts/marker/backgroundcolor/) { get; set; } | Représente la couleur d'arrière-plan du marqueur dans un graphique en ligne, un graphique de dispersion ou un graphique radar. |
| [BackgroundColorSetType](../../aspose.cells.charts/marker/backgroundcolorsettype/) { get; set; } | Obtient ou définit le type de jeu de couleurs d'arrière-plan du marqueur. |
| [Border](../../aspose.cells.charts/marker/border/) { get; } | Obtient le [`border`](../../aspose.cells.drawing/line/). |
| [ForegroundColor](../../aspose.cells.charts/marker/foregroundcolor/) { get; set; } | Représente la couleur de premier plan du marqueur dans un graphique en ligne, un graphique de dispersion ou un graphique radar. |
| [ForegroundColorSetType](../../aspose.cells.charts/marker/foregroundcolorsettype/) { get; set; } | Obtient ou définit le type de jeu de couleur de premier plan du marqueur. |
| [MarkerSize](../../aspose.cells.charts/marker/markersize/) { get; set; } | Représente la taille du marqueur en unité de points. S'applique aux graphiques en ligne, aux graphiques en nuage de points ou aux graphiques radar. |
| [MarkerSizePx](../../aspose.cells.charts/marker/markersizepx/) { get; set; } | Représente la taille du marqueur en unités de pixels. S'applique aux graphiques en ligne, aux graphiques en nuage de points ou aux graphiques radar. |
| [MarkerStyle](../../aspose.cells.charts/marker/markerstyle/) { get; set; } | Représente le style du marqueur. S'applique à un graphique en ligne, un graphique en nuage de points ou un graphique radar. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MarkerDemo
    {
        public static void MarkerExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            // Obtenez la référence de la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajoutez NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B3"
            chart.NSeries.Add("A1:B3", true);

            // Accéder à la première série
            Series series = chart.NSeries[0];

            // Définir les propriétés du marqueur
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.MarkerSize = 10; // Size in points
            series.Marker.MarkerSizePx = 20; // Size in pixels
            series.Marker.ForegroundColor = Color.Red;
            series.Marker.ForegroundColorSetType = FormattingType.Custom;
            series.Marker.BackgroundColor = Color.Yellow;
            series.Marker.BackgroundColorSetType = FormattingType.Custom;

            // Enregistrez le classeur
            workbook.Save("MarkerExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


