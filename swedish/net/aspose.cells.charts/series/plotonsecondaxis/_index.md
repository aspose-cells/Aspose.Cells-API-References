---
title: "Series.PlotOnSecondAxis"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Anger om denna serie plottas på den andra värdeaxeln"
type: docs
url: /sv/net/aspose.cells.charts/series/plotonsecondaxis/
---
## Series.PlotOnSecondAxis property

Anger om denna serie plottas på den sekundära värdeaxeln.

```csharp
public bool PlotOnSecondAxis { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyPlotOnSecondAxisDemo
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

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Lägg till serier i diagrammet
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ställ in den första serien för att plottas på sekundär axel
            chart.NSeries[0].PlotOnSecondAxis = true;

            // Spara arbetsboken
            workbook.Save("SeriesPropertyPlotOnSecondAxisDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


