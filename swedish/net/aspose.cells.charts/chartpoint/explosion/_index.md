---
title: "ChartPoint.Explosion"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint egenskap. Avståndet för en öppen pajskiva från mitten av pajdiagrammet uttrycks som en procentandel av pajens diameter"
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/explosion/
---
## ChartPoint.Explosion property

Avståndet för ett öppet pajsegment från centrum av pajdiagrammet uttrycks som en procentandel av pajens diameter.

```csharp
public int Explosion { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyExplosionDemo
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

            // Lägg till ett pajdiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Få åtkomst till den första diagrampunkten och sätt explosionen
            ChartPoint point = chart.NSeries[0].Points[0];
            point.Explosion = 15; // Set explosion distance (15 points)

            // Spara arbetsboken
            workbook.Save("ChartPointExplosionDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


