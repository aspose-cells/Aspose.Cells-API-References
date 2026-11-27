---
title: "Walls.CenterY"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Walls-egenskap. Hämtar y-koordinaten för det vänstra nedre hörnet av väggens centrum i enheter av 1/4000 av diagrammets höjd efter att ha anropat metoden Chart.Calculate."
type: docs
url: /sv/net/aspose.cells.charts/walls/centery/
---
## Walls.CenterY property

Hämtar y-koordinaten för vänster‑nedre hörnet av väggens centrum i enheter av 1/4000 av diagrammets höjd efter att ha anropat metoden Chart.Calculate().

```csharp
public int CenterY { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyCenterYDemo
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

            // Beräkna diagrammet för att uppdatera egenskaper.
            chart.Calculate();

            // Åtkomst till väggar och demonstrera CenterY-egenskapen.
            Aspose.Cells.Charts.Walls walls = chart.Walls;
            Console.WriteLine("Wall CenterY position: " + walls.CenterY);

            // Spara arbetsboken
            workbook.Save("WallsCenterYDemo.xlsx");
        }
    }
}
```

### Se även

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


