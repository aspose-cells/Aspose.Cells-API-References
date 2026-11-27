---
title: "Walls.Height"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Walls-egenskap. Hämtar höjden från topp till botten i enheter av 1/4000 av diagrammets höjd efter anrop av metoden Chart.Calculate."
type: docs
url: /sv/net/aspose.cells.charts/walls/height/
---
## Walls.Height property

Hämtar höjden från topp till botten i enheter av 1/4000 av diagrammets höjd efter anrop av metoden Chart.Calculate().

```csharp
public int Height { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyHeightDemo
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

            // Åtkomst till väggar och demonstrera Height-egenskapen.
            Walls walls = chart.Walls;
            Console.WriteLine("Wall Height: " + walls.Height);
            Console.WriteLine("Wall Height in Pixels: " + walls.HeightPx);

            // Ändra diagramområdets storlek istället för direkt Height-egenskap.
            chart.ChartObject.Height = 400;
            chart.Calculate();
            Console.WriteLine("After resizing - Wall Height: " + walls.Height);
            Console.WriteLine("After resizing - Wall Height in Pixels: " + walls.HeightPx);

            workbook.Save("WallsHeightDemo.xlsx");
        }
    }
}
```

### Se även

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


