---
title: "Series.HasSeriesLines"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series‑egenskap. Sant om ett staplat kolumndiagram eller staplat stapeldiagram har serielinjer eller om ett Pie of Pie‑diagram eller Bar of Pie‑diagram har anslutningslinjer mellan de två sektionerna. Gäller endast staplade kolumndiagram, staplade stapeldiagram, Pie of Pie‑diagram eller Bar of Pie‑diagram."
type: docs
url: /sv/net/aspose.cells.charts/series/hasserieslines/
---
## Series.HasSeriesLines property

Sant om ett staplat kolumndiagram eller stapeldiagram har serielinjer eller om ett Pie of Pie-diagram eller Bar of Pie-diagram har anslutningslinjer mellan de två sektionerna. Gäller endast staplade kolumndiagram, stapeldiagram, Pie of Pie-diagram eller Bar of Pie-diagram.

```csharp
public bool HasSeriesLines { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasSeriesLinesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Q3");

            // Lägg till ett staplat kolumndiagram
            int chartIndex = worksheet.Charts.Add(ChartType.ColumnStacked, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till seriedata
            chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "C1:C3";

            // Åtkomst till den första serien
            Series series = chart.NSeries[0];
            
            // Demonstrera HasSeriesLines‑egenskapen
            series.HasSeriesLines = true; // Enable series lines
            
            // Spara arbetsboken
            workbook.Save("SeriesHasSeriesLinesDemo.xlsx");
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


