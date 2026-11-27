---
title: "Enum TickLabelPositionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.TickLabelPositionType enum. Representerar positionstypen för tickmarkeringarnas etiketter på den angivna axeln"
type: docs
url: /sv/net/aspose.cells.charts/ticklabelpositiontype/
---
## TickLabelPositionType enumeration

Representerar positionstypen för tick‑mark‑etiketterna på den angivna axeln.

```csharp
public enum TickLabelPositionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| High | `0` | Positionstypen är hög. |
| Low | `1` | Positionstypen är låg. |
| NextToAxis | `2` | Positionstypen är bredvid axeln. |
| None | `3` | Positionstypen är ingen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelPositionTypeDemo
    {
        public static void TickLabelPositionTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till NSeries (diagramdatakälla) till diagrammet som sträcker sig från cellen "A1" till "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Åtkomst till kategoriaxeln
            Axis categoryAxis = chart.CategoryAxis;
            
            // Ställ in tick-etikettens position till High
            categoryAxis.TickLabelPosition = TickLabelPositionType.High;
            
            // Spara arbetsboken
            workbook.Save("TickLabelPositionTypeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


