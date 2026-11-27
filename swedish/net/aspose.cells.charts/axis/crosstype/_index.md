---
title: "Axis.CrossType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis-egenskap. Representerar CrossType på den angivna axeln där den andra axeln korsar"
type: docs
url: /sv/net/aspose.cells.charts/axis/crosstype/
---
## Axis.CrossType property

Representerar `CrossType` på den angivna axeln där den andra axeln korsar.

```csharp
public CrossType CrossType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyCrossTypeDemo
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

            // Skapa diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Konfigurera värdeaxeln
            chart.ValueAxis.MaxValue = 200;
            chart.ValueAxis.MinValue = 0;
            chart.ValueAxis.MajorUnit = 25;
            
            // Demonstrera CrossType‑egenskapen
            chart.ValueAxis.CrossType = CrossType.Maximum;

            workbook.Save("AxisPropertyCrossTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [CrossType](../../crosstype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


