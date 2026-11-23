---
title: "Walls.WidthPx"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Walls. Obtient la largeur de gauche à droite en unités de pixels après l'appel de la méthode Chart.Calculate"
type: docs
url: /fr/net/aspose.cells.charts/walls/widthpx/
---
## Walls.WidthPx property

Obtient la largeur de gauche à droite en unités de pixels après avoir appelé la méthode Chart.Calculate().

```csharp
public int WidthPx { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyWidthPxDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Calculate();

            // Obtenir les murs et démontrer la propriété WidthPx
            Walls walls = chart.Walls;
            Console.WriteLine("Wall width in pixels: " + walls.WidthPx);

            // Enregistrer le classeur
            workbook.Save("WallsWidthPxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


