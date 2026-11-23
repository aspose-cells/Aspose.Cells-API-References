---
title: "Walls.Width"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Walls. Obtient la largeur de gauche à droite en unités de 1/4000 de la largeur du graphique après l'appel de la méthode Chart.Calculate"
type: docs
url: /fr/net/aspose.cells.charts/walls/width/
---
## Walls.Width property

Obtient la largeur de gauche à droite en unités de 1/4000 de la largeur du graphique après l'appel de la méthode Chart.Calculate().

```csharp
public int Width { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyWidthDemo
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

            // Ajouter un graphique 3D
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column3D, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculer le graphique
            chart.Calculate();

            // Accéder aux murs et démontrer la propriété Width
            Aspose.Cells.Charts.Walls walls = chart.Walls;
            Console.WriteLine("Wall Width: " + walls.Width);
            Console.WriteLine("Wall Width in Pixels: " + walls.WidthPx);

            // Enregistrez le classeur
            workbook.Save("WallsWidthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


