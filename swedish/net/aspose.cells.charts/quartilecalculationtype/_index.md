---
title: "Enum QuartileCalculationType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.QuartileCalculationType enum. Representerar kvartilberäkningsmetoder"
type: docs
url: /sv/net/aspose.cells.charts/quartilecalculationtype/
---
## QuartileCalculationType enumeration

Representerar kvartilberäkningsmetoder.

```csharp
public enum QuartileCalculationType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Exclusive | `0` | Kvartilberäkningen inkluderar medianen när datasettet delas in i kvartiler. |
| Inclusive | `1` | Kvartilberäkningen exkluderar medianen när datasettet delas in i kvartiler. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class QuartileCalculationTypeDemo
    {
        public static void QuartileCalculationTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 7, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till serier i diagrammet
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Åtkomst till seriens layoutegenskaper
            SeriesLayoutProperties layoutProperties = chart.NSeries[0].LayoutProperties;

            // Ställ in kvartilberäkningstypen
            layoutProperties.QuartileCalculation = QuartileCalculationType.Exclusive;

            // Spara arbetsboken
            workbook.Save("QuartileCalculationTypeExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


