---
title: "Series.Shadow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Sant om serien har en skugga."
type: docs
url: /sv/net/aspose.cells.charts/series/shadow/
---
## Series.Shadow property

Sant om serien har en skugga.

```csharp
public bool Shadow { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyShadowDemo
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

            // Skapa diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Åtkomst till den första serien och aktivera skugga.
            Series series = chart.NSeries[0];
            series.Shadow = true;

            // Spara och ladda om för att verifiera
            workbook.Save("output.xlsx");
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Series loadedSeries = loadedWorkbook.Worksheets[0].Charts[0].NSeries[0];
            Console.WriteLine("Shadow enabled: " + loadedSeries.Shadow);
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


