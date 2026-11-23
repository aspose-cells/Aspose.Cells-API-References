---
title: "Enum ChartMarkerType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Charts.ChartMarkerType. Représente le style de repère dans un graphique en courbes, un graphique en nuage de points ou un graphique radar"
type: docs
url: /fr/net/aspose.cells.charts/chartmarkertype/
---
## ChartMarkerType enumeration

Représente le style de marqueur dans un graphique en ligne, un nuage de points ou un graphique radar.

```csharp
public enum ChartMarkerType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Automatic | `0` | Repères automatiques. |
| Circle | `1` | Repères circulaires. |
| Dash | `2` | Repères à barre longue |
| Diamond | `3` | Repères en forme de losange. |
| Dot | `4` | Repères à barre courte. |
| None | `5` | Pas de repères. |
| SquarePlus | `6` | Repères carrés avec un signe plus. |
| Square | `7` | Repères carrés. |
| SquareStar | `8` | Repères carrés avec un astérisque. |
| Triangle | `9` | Marqueurs triangulaires. |
| SquareX | `10` | Marqueurs carrés avec un X. |
| Picture | `11` | Image |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartMarkerTypeDemo
    {
        public static void ChartMarkerTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajoutez la série de données au graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accéder au marqueur de la première série
            Marker marker = chart.NSeries[0].Marker;

            // Définir le style du marqueur
            marker.MarkerStyle = ChartMarkerType.Circle;

            // Définir la taille du marqueur
            marker.MarkerSize = 10;

            // Définir les couleurs de premier plan et d'arrière-plan du marqueur
            marker.ForegroundColor = Color.Red;
            marker.BackgroundColor = Color.Yellow;

            // Enregistrez le classeur
            workbook.Save("ChartMarkerTypeExample.xlsx");
            workbook.Save("ChartMarkerTypeExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


