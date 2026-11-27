---
title: "Axis.IsAutomaticMinValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis-egenskap. Indikerar om minvärdet tilldelas automatiskt"
type: docs
url: /sv/net/aspose.cells.charts/axis/isautomaticminvalue/
---
## Axis.IsAutomaticMinValue property

Indikerar om minvärdet tilldelas automatiskt

```csharp
public bool IsAutomaticMinValue { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutomaticMinValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Lägg till diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Konfigurera värdeaxeln
            Axis valueAxis = chart.ValueAxis;
            valueAxis.IsAutomaticMinValue = false;
            valueAxis.MinValue = 0;
            valueAxis.IsAutomaticMaxValue = true; // Keep max value automatic for contrast
            
            // Spara resultatet
            workbook.Save("AxisPropertyIsAutomaticMinValueDemo.xlsx");
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


