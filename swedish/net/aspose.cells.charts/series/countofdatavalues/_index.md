---
title: "Series.CountOfDataValues"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Hämtar antalet datavärden"
type: docs
url: /sv/net/aspose.cells.charts/series/countofdatavalues/
---
## Series.CountOfDataValues property

Hämtar antalet datavärden.

```csharp
public int CountOfDataValues { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyCountOfDataValuesDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            for (int i = 0; i < 4; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1); // A1:A4 with values 1-4
            }

            // Skapa ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till serier med dataområdet
            chart.NSeries.Add("A1:A4", true);
            
            // Visa antalet datavärden i den första serien
            Console.WriteLine("Count of data values in series: " + chart.NSeries[0].CountOfDataValues);
            
            // Spara arbetsboken
            workbook.Save("SeriesPropertyCountOfDataValuesDemo.xlsx");
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


