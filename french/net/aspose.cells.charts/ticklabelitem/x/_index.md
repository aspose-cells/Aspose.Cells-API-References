---
title: "TickLabelItem.X"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TickLabelItem. Coordonnées X de l'élément TickLabel comme un ratio de la largeur du graphique"
type: docs
url: /fr/net/aspose.cells.charts/ticklabelitem/x/
---
## TickLabelItem.X property

Coordonnées X de l'élément Ticklabel en tant que ratio de la largeur du graphique.

```csharp
public double X { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelItemPropertyXDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculer le graphique
            chart.Calculate();

            // Accéder aux éléments d'étiquette de repère
            Aspose.Cells.Charts.Axis axis = chart.CategoryAxis;
            Aspose.Cells.Charts.TickLabelItem[] items = axis.TickLabels.TickLabelItems;

            // Ajouter des formes à chaque position d'étiquette de repère en utilisant la propriété X
            for (int i = 0; i < items.Length; i++)
            {
                Aspose.Cells.Charts.TickLabelItem item = items[i];
                
                // Ajouter un rectangle à la position de l'étiquette de repère
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle, 
                    PlacementType.Move,
                    item.X, 
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                
                shape.Fill.SolidFill.Color = Color.LightBlue;
                shape.Line.SolidFill.Color = Color.Blue;

                // Ajouter un cercle à côté de l'étiquette de repère en utilisant la propriété X
                Shape circle = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Oval,
                    PlacementType.Move,
                    item.X + item.Width,
                    item.Y,
                    item.X + item.Width + 0.05, // Small offset
                    item.Y + item.Height);
                
                circle.Fill.SolidFill.Color = Color.Red;
            }

            // Enregistrez le classeur
            workbook.Save("TickLabelItemPropertyXDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


