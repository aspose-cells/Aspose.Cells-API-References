---
title: "Series.SecondPlotSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series‑egenskap. Returnerar eller anger storleken på den sekundära delen av antingen ett paj‑paj‑diagram eller ett stapel‑paj‑diagram som en procentsats av storleken på den primära pajen. Kan vara ett värde mellan 5 och 200"
type: docs
url: /sv/net/aspose.cells.charts/series/secondplotsize/
---
## Series.SecondPlotSize property

Returnerar eller anger storleken på den sekundära sektionen i antingen ett Pie of Pie-diagram eller ett Bar of Pie-diagram, som en procentandel av storleken på den primära pajen. Kan vara ett värde mellan 5 och 200.

```csharp
public short SecondPlotSize { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySecondPlotSizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pajdiagram
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Lägg till ett pajdiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hämta den första serien
            Series series = chart.NSeries[0];

            // Ställ in SecondPlotSize‑egenskapen (procent av pajen som ska visas i andra diagrammet)
            series.SecondPlotSize = 30; // 30% of the pie will be shown in second plot

            // Spara arbetsboken
            workbook.Save("SeriesPropertySecondPlotSizeDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


