---
title: "Enum TimeUnit"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.TimeUnit enum. Representerar basenheten för kategoriaxeln"
type: docs
url: /sv/net/aspose.cells.charts/timeunit/
---
## TimeUnit enumeration

Representerar basenheten för kategori‑axeln.

```csharp
public enum TimeUnit
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Days | `0` | Dagar |
| Months | `1` | Månader |
| Years | `2` | År |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TimeUnitDemo
    {
        public static void TimeUnitExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            // Lägg till ett nytt arbetsblad
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["B3"].PutValue(300);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till serier i diagrammet
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Ställ in kategoriaxeln för att använda tidsenheter
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.CategoryType = CategoryType.TimeScale;
            categoryAxis.BaseUnitScale = TimeUnit.Months;
            categoryAxis.MajorUnitScale = TimeUnit.Months;
            categoryAxis.MinorUnitScale = TimeUnit.Days;

            // Anpassa diagrammets utseende
            chart.Title.Text = "Sample Chart with Time Units";
            chart.ValueAxis.Title.Text = "Values";
            chart.CategoryAxis.Title.Text = "Dates";

            // Spara arbetsboken
            workbook.Save("TimeUnitExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


