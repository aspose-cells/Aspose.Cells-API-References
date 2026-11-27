---
title: "Series.HasDropLines"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Sant om diagrammet har droplinjer. Gäller endast linjediagram eller områdesdiagram"
type: docs
url: /sv/net/aspose.cells.charts/series/hasdroplines/
---
## Series.HasDropLines property

Sant om diagrammet har droplinjer. Gäller endast för linje- eller områdesdiagram.

```csharp
public bool HasDropLines { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasDropLinesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
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

            // Lägg till ett linjediagram
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till seriedata
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hämta den första serien
            Series series = chart.NSeries[0];

            // Demonstrera HasDropLines-egenskapen
            series.HasDropLines = true; // Enable drop lines
            series.Type = ChartType.Line; // Ensure it's a line chart for drop lines to be visible

            // Spara arbetsboken
            workbook.Save("SeriesHasDropLinesDemo.xlsx");
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


