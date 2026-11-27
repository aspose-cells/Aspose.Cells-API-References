---
title: "Walls.Width"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Walls‑egenskapen. Hämtar bredden från vänster till höger i enheter av 1/4000 av diagrammets bredd efter anrop av metoden Chart.Calculate."
type: docs
url: /sv/net/aspose.cells.charts/walls/width/
---
## Walls.Width property

Hämtar bredden från vänster till höger i enheter av 1/4000 av diagrammets bredd efter anrop av metoden Chart.Calculate().

```csharp
public int Width { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett 3D-diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column3D, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet
            chart.Calculate();

            // Åtkomst till väggar och demonstrera Width‑egenskapen
            Aspose.Cells.Charts.Walls walls = chart.Walls;
            Console.WriteLine("Wall Width: " + walls.Width);
            Console.WriteLine("Wall Width in Pixels: " + walls.WidthPx);

            // Spara arbetsboken
            workbook.Save("WallsWidthDemo.xlsx");
        }
    }
}
```

### Se även

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


