---
title: "Series.SplitType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series‑egenskap. Returnerar eller anger ett värde som bestämmer vilka datapunkter som ligger i den andra pajen eller stapeln i ett paj‑i‑paj‑ eller stapel‑i‑paj‑diagram"
type: docs
url: /sv/net/aspose.cells.charts/series/splittype/
---
## Series.SplitType property

Returnerar eller anger ett värde som bestämmer vilka datapunkter som finns i den andra pajen eller stapeln i ett Pie of Pie- eller Bar of Pie-diagram.

```csharp
public ChartSplitType SplitType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySplitTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Lägg till ett pajdiagram
            int chartIndex = sheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ange split‑typ för den första serien
            chart.NSeries[0].SplitType = ChartSplitType.Position;

            // Spara arbetsboken
            workbook.Save("SeriesPropertySplitTypeDemo_out.xlsx");
        }
    }
}
```

### Se även

* enum [ChartSplitType](../../chartsplittype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


