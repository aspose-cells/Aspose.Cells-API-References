---
title: "Legend.Position"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Legend-egenskap. Hämtar eller anger legenden positionstyp"
type: docs
url: /sv/net/aspose.cells.charts/legend/position/
---
## Legend.Position property

Hämtar eller anger förklaringens positionstyp.

```csharp
public LegendPositionType Position { get; set; }
```

### Anmärkningar

Standardpositionen är höger. Om legenden är på vänster eller högra sidan av diagrammet kommer inställning av Legend.X-egenskapen inte att ha någon effekt. Om legenden är på över- eller undersidan av diagrammet kommer inställning av Legend.Y-egenskapen inte att ha någon effekt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendPropertyPositionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Ange legendposition
            chart.Legend.Position = LegendPositionType.Left;

            // Spara arbetsboken
            workbook.Save("LegendPositionDemo.xlsx");
        }
    }
}
```

### Se även

* enum [LegendPositionType](../../legendpositiontype/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


