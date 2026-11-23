---
title: "Walls.Depth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Walls. Obtient la profondeur de l'avant à l'arrière en unités de 1/4000 de la largeur du graphique après l'appel de la méthode Chart.Calculate"
type: docs
url: /fr/net/aspose.cells.charts/walls/depth/
---
## Walls.Depth property

Obtient la profondeur avant‑arrière en unités de 1/4000 de la largeur du graphique après l'appel de la méthode Chart.Calculate().

```csharp
public int Depth { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyDepthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            Walls walls = chart.Walls;
            Console.WriteLine("Wall Depth: " + walls.Depth);

            workbook.Save("WallsDepthExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


