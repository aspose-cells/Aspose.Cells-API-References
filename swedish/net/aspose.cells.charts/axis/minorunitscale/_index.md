---
title: "Axis.MinorUnitScale"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis-egenskap. Representerar huvudenhetsskalan för kategoriaxeln"
type: docs
url: /sv/net/aspose.cells.charts/axis/minorunitscale/
---
## Axis.MinorUnitScale property

Anger huvudenhetsskalan för kategori‑axeln.

```csharp
public TimeUnit MinorUnitScale { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMinorUnitScaleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempel på tidsbaserad data
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(DateTime.Now.AddMonths(i - 2));
                worksheet.Cells[$"B{i}"].PutValue(i * 100);
            }

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Konfigurera kategoriaxeln som tidskala
            chart.CategoryAxis.CategoryType = CategoryType.TimeScale;
            chart.CategoryAxis.MinorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MinorUnit = 2;

            // Spara arbetsboken
            workbook.Save("AxisPropertyMinorUnitScaleDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


