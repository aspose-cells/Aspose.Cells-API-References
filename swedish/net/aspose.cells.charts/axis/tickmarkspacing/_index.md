---
title: "Axis.TickMarkSpacing"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis‑egenskap. Returnerar eller anger antalet kategorier eller serier mellan tick‑markeringar. Gäller endast kategori‑ och serieaxlar"
type: docs
url: /sv/net/aspose.cells.charts/axis/tickmarkspacing/
---
## Axis.TickMarkSpacing property

Returnerar eller anger antalet kategorier eller serier mellan tick‑markeringar. Gäller endast för kategori‑ och serieaxlar.

```csharp
public int TickMarkSpacing { get; set; }
```

### Anmärkningar

Numret måste vara mellan 1 och 31999.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTickMarkSpacingDemo
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

            // Konfigurera värdeaxeln med TickMarkSpacing
            Axis valueAxis = chart.ValueAxis;
            valueAxis.MinValue = 0;
            valueAxis.MaxValue = 200;
            valueAxis.MajorUnit = 25;
            valueAxis.MinorUnit = 5;
            valueAxis.TickMarkSpacing = 2; // Setting tick mark spacing
            
            // Konfigurera kategori‑axeln med TickMarkSpacing
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.TickMarkSpacing = 1; // Setting tick mark spacing

            workbook.Save("AxisTickMarkSpacingDemo.xlsx");
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


