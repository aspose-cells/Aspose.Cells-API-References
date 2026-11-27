---
title: "Series.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Hämtar eller anger namnet på dataserien"
type: docs
url: /sv/net/aspose.cells.charts/series/name/
---
## Series.Name property

Hämtar eller anger namnet på dataserien.

```csharp
public string Name { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Series Name");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["C2"].PutValue(30);
            
            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till serier i diagrammet
            chart.NSeries.Add("A2:C2", true);
            
            // Demonstrera användning av Name‑egenskapen
            // 1. Referensnamn till en cell
            chart.NSeries[0].Name = "=A1";
            
            // 2. Ange en sträng som namn
            chart.NSeries[0].Name = "First Series";
            
            // Spara arbetsboken
            workbook.Save("SeriesPropertyNameDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


