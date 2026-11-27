---
title: "Class ChartCalculateOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.ChartCalculateOptions class. Representerar alternativen för att beräkna ett diagram"
type: docs
url: /sv/net/aspose.cells.charts/chartcalculateoptions/
---
## ChartCalculateOptions class

Representerar alternativen för att beräkna ett diagram.

```csharp
public class ChartCalculateOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [ChartCalculateOptions](chartcalculateoptions/)() | Skapar alternativen för att beräkna diagrammet. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [UpdateAllPoints](../../aspose.cells.charts/chartcalculateoptions/updateallpoints/) { get; set; } | Huruvida alla datapunkter ska uppdateras vid diagramberäkning. Standard: False. När du vill hämta värdet för varje datapunkt i diagrammet specifikt, sätt den till true. Om denna parameter är satt till True kan nya datapunkter genereras när diagrammet beräknas. Detta kan göra Excel-filen större. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCalculateOptionsDemo
    {
        public static void ChartCalculateOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange dataintervallet för diagrammet
            chart.SetChartDataRange("A1:B4", true);

            // Skapa en instans av ChartCalculateOptions
            ChartCalculateOptions options = new ChartCalculateOptions
            {
                UpdateAllPoints = true // Set the property to update all data points
            };

            // Beräkna diagrammet med de angivna alternativen
            chart.Calculate(options);

            // Spara arbetsboken
            workbook.Save("ChartCalculateOptionsExample.xlsx");
            workbook.Save("ChartCalculateOptionsExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


