---
title: "Walls.CenterX"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Walls-Eigenschaft. Gibt die x‑Koordinate der linken unteren Ecke des Wandzentrums in Einheiten von 1/4000 der Diagrammbreite zurück, nachdem die Methode Chart.Calculate aufgerufen wurde."
type: docs
url: /de/net/aspose.cells.charts/walls/centerx/
---
## Walls.CenterX property

Liest die x‑Koordinate der linken unteren Ecke des Wandzentrums in Einheiten von 1/4000 der Diagrammbreite nach Aufruf der Methode Chart.Calculate().

```csharp
public int CenterX { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyCenterXDemo
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

            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Calculate();

            Walls walls = chart.Walls;
            Console.WriteLine("Wall CenterX position: " + walls.CenterX);

            workbook.Save("WallsCenterXExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


