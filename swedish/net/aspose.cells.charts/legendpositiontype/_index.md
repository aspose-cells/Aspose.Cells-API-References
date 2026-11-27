---
title: "Enum LegendPositionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.LegendPositionType enum. Enumererar typerna av legendposition"
type: docs
url: /sv/net/aspose.cells.charts/legendpositiontype/
---
## LegendPositionType enumeration

Enumererar legendens positionstyper.

```csharp
public enum LegendPositionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Bottom | `0` | Visar legenden längst ner i diagrammets plotområde. |
| Corner | `1` | Visar legenden i hörnet av diagrammets plotområde. |
| Left | `4` | Visar legenden till vänster om diagrammets plotområde. |
| NotDocked | `7` | Indikerar att legenden inte är dockad. |
| Right | `3` | Visar legenden till höger om diagrammets plotområde. |
| Top | `2` | Visar legenden högst upp i diagrammets plotområde. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendPositionTypeDemo
    {
        public static void LegendPositionTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            Cells cells = sheet.Cells;
            cells[0, 1].PutValue("Income");
            cells[1, 0].PutValue("Company A");
            cells[2, 0].PutValue("Company B");
            cells[3, 0].PutValue("Company C");
            cells[1, 1].PutValue(10000);
            cells[2, 1].PutValue(20000);
            cells[3, 1].PutValue(30000);

            // Lägg till ett stapeldiagram i kalkylbladet
            int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Åtkomst till diagrammets förklaring
            Legend legend = chart.Legend;

            // Ställ in legendens position till vänster om diagrammet
            legend.Position = LegendPositionType.Left;

            // Ange ytterligare egenskaper för legenden
            legend.Y = 1500;
            legend.Width = 50;
            legend.Height = 50;

            // Spara arbetsboken
            workbook.Save("LegendPositionTypeExample.xlsx");
            workbook.Save("LegendPositionTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


