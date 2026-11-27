---
title: "Series.XValues"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Representerar X‑värdena för denna diagramserie"
type: docs
url: /sv/net/aspose.cells.charts/series/xvalues/
---
## Series.XValues property

Representerar X‑värdena för denna diagramserie.

```csharp
public string XValues { get; set; }
```

### Anmärkningar

Endast för spridnings- och bubbeldiagram. Använd [`CategoryData`](../../seriescollection/categorydata/) för andra diagramtyper. [`CategoryValues`](../categoryvalues/) används för att hämta de faktiska kategorivärdena för denna serie.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyXValuesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            var workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["C1"].PutValue("Series 2");
            
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i+1, 0].PutValue(i+1); // X values 1-5
                worksheet.Cells[i+1, 1].PutValue((i+1)*2); // Series 1 values
                worksheet.Cells[i+1, 2].PutValue((i+1)*3); // Series 2 values
            }

            // Lägg till ett spridningsdiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till serie med XValues och Values
            int seriesIndex = chart.NSeries.Add("B2:B6", false);
            Series series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A6"; // Demonstrating XValues property
            series.Name = "Series 1";

            seriesIndex = chart.NSeries.Add("C2:C6", false);
            series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A6"; // Demonstrating XValues property again
            series.Name = "Series 2";

            // Spara arbetsboken
            workbook.Save("SeriesXValuesDemo.xlsx");
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


