---
title: "Axis.IsDisplayUnitLabelShown"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis-egenskap. Representerar om visningsenhetsetiketten visas på den angivna axeln"
type: docs
url: /sv/net/aspose.cells.charts/axis/isdisplayunitlabelshown/
---
## Axis.IsDisplayUnitLabelShown property

Anger om enheten för visningsetikett visas på den angivna axeln.

```csharp
public bool IsDisplayUnitLabelShown { get; set; }
```

### Anmärkningar

Det förvalda värdet är True. Fungerar endast när [`DisplayUnit`](../displayunit/) inte är None.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsDisplayUnitLabelShownDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Exempeldata
            worksheet.Cells["A1"].PutValue(500000);
            worksheet.Cells["A2"].PutValue(1000000);
            worksheet.Cells["A3"].PutValue(1500000);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Skapa diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            
            // Konfigurera visningsenhet och etikettens synlighet
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Millions;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            workbook.Save("AxisPropertyIsDisplayUnitLabelShownDemo.xlsx");
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


