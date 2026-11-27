---
title: "Enum MsoArrowheadLength"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.MsoArrowheadLength enum. Enumererar linjeändans bredd för formens kantlinje"
type: docs
url: /sv/net/aspose.cells.drawing/msoarrowheadlength/
---
## MsoArrowheadLength enumeration

Enumererar linjeändans bredd för formens kantlinje.

```csharp
public enum MsoArrowheadLength
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Short | `0` | Kort linjeändslängd |
| Medium | `1` | Mellanlinjeändslängd |
| Long | `2` | Lång linjeändslängd |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoArrowheadLengthDemo
    {
        public static void MsoArrowheadLengthExample()
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
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataintervall
            chart.SetChartDataRange("A1:B4", true);

            // Skapa en linjeform för diagrammet
            Line line = chart.Line;

            // Ställ in pilspetslängderna
            line.BeginArrowLength = MsoArrowheadLength.Medium;
            line.EndArrowLength = MsoArrowheadLength.Long;

            // Skriv ut pilspetslängderna
            Console.WriteLine("Begin Arrowhead Length: " + line.BeginArrowLength);
            Console.WriteLine("End Arrowhead Length: " + line.EndArrowLength);

            // Spara arbetsboken
            workbook.Save("MsoArrowheadLengthExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


