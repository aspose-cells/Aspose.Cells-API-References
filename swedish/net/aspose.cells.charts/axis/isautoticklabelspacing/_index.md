---
title: "Axis.IsAutoTickLabelSpacing"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis-egenskap. Anger om avståndet mellan tick-etiketter är automatiskt"
type: docs
url: /sv/net/aspose.cells.charts/axis/isautoticklabelspacing/
---
## Axis.IsAutoTickLabelSpacing property

Anger om avståndet för tick‑etiketten är automatiskt

```csharp
public bool IsAutoTickLabelSpacing { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutoTickLabelSpacingDemo
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
            valueAxis.IsAutoTickLabelSpacing = true; // Core property demonstration
            
            // Konfigurera kategoriaxeln
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.IsAutoTickLabelSpacing = false; // Core property demonstration
            categoryAxis.TickLabelSpacing = 2;

            workbook.Save("AxisPropertyIsAutoTickLabelSpacingDemo.xlsx");
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


