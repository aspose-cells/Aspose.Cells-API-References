---
title: "Classe TickLabelItem"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Charts.TickLabelItem. Représente une étiquette de repère dans le graphique"
type: docs
url: /fr/net/aspose.cells.charts/ticklabelitem/
---
## TickLabelItem class

Représente une étiquette de graduation dans le graphique.

```csharp
public class TickLabelItem
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Height](../../aspose.cells.charts/ticklabelitem/height/) { get; } | Hauteur de l'élément Ticklabel en tant que ratio de la hauteur du graphique. |
| [Width](../../aspose.cells.charts/ticklabelitem/width/) { get; } | Largeur de l'élément Ticklabel en tant que ratio de la largeur du graphique. |
| [X](../../aspose.cells.charts/ticklabelitem/x/) { get; } | Coordonnées X de l'élément Ticklabel en tant que ratio de la largeur du graphique. |
| [Y](../../aspose.cells.charts/ticklabelitem/y/) { get; } | Coordonnées Y de l'élément Ticklabel en tant que ratio de la hauteur du graphique. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartsClassTickLabelItemDemo
    {
        public static void Run()
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

            // Ajouter un graphique en colonnes
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculer le graphique
            chart.Calculate();

            // Accéder aux étiquettes de repère de l'axe des catégories
            Axis axis = chart.CategoryAxis;
            TickLabelItem[] tickLabelItems = axis.TickLabels.TickLabelItems;

            // Ajouter des formes pour marquer chaque position d'étiquette de repère
            foreach (TickLabelItem item in tickLabelItems)
            {
                // Ajouter un rectangle autour de l'étiquette de repère
                Shape rectangle = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle,
                    PlacementType.Move,
                    item.X,
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                rectangle.Fill.SolidFill.Transparency = 1;
                rectangle.Line.SolidFill.Color = Color.Blue;

                // Ajouter un cercle à côté de l'étiquette de repère
                Shape circle = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Oval,
                    PlacementType.Move,
                    item.X + item.Width,
                    item.Y,
                    item.X + item.Width + item.Height,
                    item.Y + item.Height);
                circle.Fill.SolidFill.Color = Color.Red;
            }

            // Enregistrez le classeur
            workbook.Save("TickLabelItemDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


