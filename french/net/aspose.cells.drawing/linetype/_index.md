---
title: "Enum LineType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.LineType enum. Énumère le type de bordure de Picture ou de ligne de Chart"
type: docs
url: /fr/net/aspose.cells.drawing/linetype/
---
## LineType enumeration

Énumère le type de bordure de [`Picture`](../picture/) ou de ligne de [`Chart`](../../aspose.cells.charts/chart/).

```csharp
public enum LineType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| DarkGray | `6` | Représente une ligne gris foncé. |
| Dash | `1` | Représente une ligne en tirets. |
| DashDot | `3` | Représente une ligne tiret-point |
| DashDotDot | `4` | Représente une ligne tiret-point-point. |
| Dot | `2` | Représente une ligne pointillée. |
| LightGray | `8` | Représente une ligne gris clair. |
| MediumGray | `7` | Représente une ligne gris moyen. |
| Solid | `0` | Représente une ligne pleine. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class LineTypeDemo
    {
        public static void LineTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.SetChartDataRange("A1:B4", true);

            // Accéder à l'axe de catégorie principal
            Axis categoryAxis = chart.CategoryAxis;

            // Définir le type de ligne pour la ligne d'axe
            categoryAxis.AxisLine.Style = LineType.DashDot;

            // Définir la couleur de la ligne d'axe
            categoryAxis.AxisLine.Color = Color.Blue;

            // Accéder à l'axe de valeur principal
            Axis valueAxis = chart.ValueAxis;

            // Définir le type de ligne pour les principales lignes de grille
            valueAxis.MajorGridLines.Style = LineType.Dot;

            // Définir la couleur des principales lignes de grille
            valueAxis.MajorGridLines.Color = Color.Red;

            // Enregistrez le classeur
            workbook.Save("LineTypeExample.xlsx");

            // Afficher les résultats
            Console.WriteLine("Chart created with custom line types for axis and gridlines.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


