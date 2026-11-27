---
title: "Walls.WidthPx"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Walls‑egenskapen. Hämtar bredden från vänster till höger i pixelenheter efter anrop av metoden Chart.Calculate."
type: docs
url: /sv/net/aspose.cells.charts/walls/widthpx/
---
## Walls.WidthPx property

Hämtar bredden från vänster till höger i pixelenheter efter att ha anropat metoden Chart.Calculate().

```csharp
public int WidthPx { get; }
```

### Exempel

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

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till 3D-diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Calculate();

            // Hämta väggar och demonstrera WidthPx‑egenskapen
            Walls walls = chart.Walls;
            Console.WriteLine("Wall width in pixels: " + walls.WidthPx);

            // Spara arbetsbok
            workbook.Save("WallsWidthPxDemo.xlsx");
        }
    }
}
```

### Se även

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


