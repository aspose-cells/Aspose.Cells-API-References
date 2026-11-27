---
title: "Enum TickMarkType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.TickMarkType enum. Representerar tick mark-typen för den angivna axeln"
type: docs
url: /sv/net/aspose.cells.charts/tickmarktype/
---
## TickMarkType enumeration

Representerar tick‑mark‑typen för den angivna axeln.

```csharp
public enum TickMarkType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Cross | `0` | Tick mark-typen är Cross. |
| Inside | `1` | Tick mark-typen är Inside. |
| None | `2` | Tick mark-typen är None. |
| Outside | `3` | Tick mark-typen är Outside |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickMarkTypeDemo
    {
        public static void TickMarkTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
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

            // Åtkomst till värdeaxeln i diagrammet
            Axis valueAxis = chart.ValueAxis;

            // Ställ in huvud-tick mark-typen till Cross
            valueAxis.MajorTickMark = TickMarkType.Cross;

            // Ställ in sekundär-tick mark-typen till Inside
            valueAxis.MinorTickMark = TickMarkType.Inside;

            // Ange det maximala värdet för värdeaxeln
            valueAxis.MaxValue = 200;

            // Ange det minsta värdet för värdeaxeln
            valueAxis.MinValue = 0;

            // Ange huvudenheten
            valueAxis.MajorUnit = 25;

            // Spara arbetsboken
            workbook.Save("TickMarkTypeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


