---
title: "Series.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Hämtar eller anger en dataserietyp"
type: docs
url: /sv/net/aspose.cells.charts/series/type/
---
## Series.Type property

Hämtar eller anger en dataserietyp.

```csharp
public ChartType Type { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyTypeDemo
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

            // Lägg till ett staplat kolumndiagram
            int chartIndex = worksheet.Charts.Add(ChartType.ColumnStacked, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Verifiera och skriv ut serietypen
            foreach (Series series in chart.NSeries)
            {
                Console.WriteLine("Series Type: " + series.Type);
            }
        }
    }
}
```

### Se även

* enum [ChartType](../../charttype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


