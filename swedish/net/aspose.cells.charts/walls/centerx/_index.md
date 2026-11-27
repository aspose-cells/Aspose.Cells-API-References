---
title: "Walls.CenterX"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Walls-egenskap. Hämtar x-koordinaten för det vänstra nedre hörnet av väggens centrum i enheter av 1/4000 av diagrammets bredd efter anrop av metoden Chart.Calculate."
type: docs
url: /sv/net/aspose.cells.charts/walls/centerx/
---
## Walls.CenterX property

Hämtar x-koordinaten för vänster‑nedre hörnet av väggens centrum i enheter av 1/4000 av diagrammets bredd efter anrop av metoden Chart.Calculate().

```csharp
public int CenterX { get; }
```

### Exempel

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

### Se även

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


