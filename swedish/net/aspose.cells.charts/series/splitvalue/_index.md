---
title: "Series.SplitValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Returnerar eller anger ett värde som ska användas för att bestämma vilka datapunkter som är i den andra pajen eller stapeln i ett paj‑i‑paj‑ eller stapel‑i‑paj‑diagram"
type: docs
url: /sv/net/aspose.cells.charts/series/splitvalue/
---
## Series.SplitValue property

Returnerar eller anger ett värde som ska användas för att bestämma vilka datapunkter som finns i den andra pajen eller stapeln på ett paj‑av‑paj‑ eller stapel‑av‑paj‑diagram.

```csharp
public double SplitValue { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySplitValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["A5"].PutValue("Grape");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(10);
            worksheet.Cells["B5"].PutValue(50);

            // Lägg till ett pajdiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Ange delningstyp och värde
            chart.NSeries[0].SplitType = ChartSplitType.Custom;
            chart.NSeries[0].SplitValue = 20; // Split points with value <= 20

            // Spara arbetsboken
            workbook.Save("SeriesPropertySplitValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


