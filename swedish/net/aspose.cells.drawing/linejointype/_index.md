---
title: "Enum LineJoinType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.LineJoinType enum. Representerar sammanfogningsstilarna för en linje"
type: docs
url: /sv/net/aspose.cells.drawing/linejointype/
---
## LineJoinType enumeration

Representerar sammanfogningsstilar för en linje.

```csharp
public enum LineJoinType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Round | `0` | Rund fog |
| Bevel | `1` | Fasfog |
| Miter | `2` | Snedfog |
| None | `3` | Ingen fog |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LineJoinTypeDemo
    {
        public static void LineJoinTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataintervall
            chart.SetChartDataRange("A1:B4", true);

            // Åtkomst till den primära värdeaxeln
            Axis valueAxis = chart.ValueAxis;

            // Åtkomst till linjeformatet för de viktigaste rutnätslinjerna
            Line majorGridLines = valueAxis.MajorGridLines;

            // Ställ in fogtypen för linjen
            majorGridLines.JoinType = LineJoinType.Round;

            // Skriv ut fogtypen
            Console.WriteLine("Line Join Type: " + majorGridLines.JoinType);

            // Spara arbetsboken
            workbook.Save("LineJoinTypeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


