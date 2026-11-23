---
title: "TickLabelItem.Y"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TickLabelItem. Coordonnées Y de l'élément TickLabel comme un ratio de la hauteur du graphique"
type: docs
url: /fr/net/aspose.cells.charts/ticklabelitem/y/
---
## TickLabelItem.Y property

Coordonnées Y de l'élément Ticklabel en tant que ratio de la hauteur du graphique.

```csharp
public double Y { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelItemPropertyYDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Ajouter un graphique en colonnes
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            
            // Définir les données de l'axe des catégories en utilisant NSERIES au lieu de CategoryData
            chart.NSeries.CategoryData = "A1:A3";

            // Calculer le graphique pour garantir que les étiquettes de repère sont générées
            chart.Calculate();

            // Obtenir les éléments d'étiquette de repère de l'axe des catégories
            Aspose.Cells.Charts.TickLabelItem[] tickLabelItems = chart.CategoryAxis.TickLabels.TickLabelItems;

            // Démontrer l'utilisation de la propriété Y en ajoutant des formes alignées avec les étiquettes de repère
            for (int i = 0; i < tickLabelItems.Length; i++)
            {
                Aspose.Cells.Charts.TickLabelItem item = tickLabelItems[i];
                
                // Ajouter un rectangle à chaque position Y d'étiquette de repère
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle, 
                    PlacementType.Move,
                    item.X,
                    item.Y, // Using the Y property of TickLabelItem
                    item.X + 0.05, // Small width
                    item.Y + 0.02); // Small height
                
                shape.Fill.SolidFill.Color = Color.FromArgb(100, 0, 255, 0); // Semi-transparent green
                shape.Line.SolidFill.Color = Color.Black;
            }

            // Enregistrez le classeur
            workbook.Save("TickLabelItemPropertyYDemo_Output.xlsx");
        }
    }
}
```

### Voir aussi

* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


