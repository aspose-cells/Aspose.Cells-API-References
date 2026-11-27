---
title: "Axis.BaseUnitScale"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis property. Representerar basenhetsskalan för kategoriaxeln"
type: docs
url: /sv/net/aspose.cells.charts/axis/baseunitscale/
---
## Axis.BaseUnitScale property

Representerar basenhetsskalan för kategoriaxeln.

```csharp
public TimeUnit BaseUnitScale { get; set; }
```

### Anmärkningar

Gäller endast när egenskapen CategoryType är inställd på TimeScale.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyBaseUnitScaleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells[$"A{i}"].PutValue(DateTime.Now.AddDays(i));
                sheet.Cells[$"B{i}"].PutValue(i * 100);
            }

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Ställ in basenhetsskalan för kategoriaxeln
            chart.CategoryAxis.BaseUnitScale = TimeUnit.Months;

            // Spara arbetsboken
            workbook.Save("AxisPropertyBaseUnitScaleDemo_out.xlsx");
        }
    }
}
```

### Se även

* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


