---
title: "Enum MsoArrowheadWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.MsoArrowheadWidth enum. Enumererar linjeändans bredd för formens kantlinje"
type: docs
url: /sv/net/aspose.cells.drawing/msoarrowheadwidth/
---
## MsoArrowheadWidth enumeration

Enumererar linjeändans bredd för formens kantlinje.

```csharp
public enum MsoArrowheadWidth
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Narrow | `0` | Kort linjeändbredd. |
| Medium | `1` | Mellanlinjeändbredd. |
| Wide | `2` | Bred linjeändbredd. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class MsoArrowheadWidthDemo
    {
        public static void MsoArrowheadWidthExample()
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

            // Skapa en linjeform för diagrammet
            Line line = chart.Line;

            // Ställ in pilspetsstilar och -bredder
            line.BeginType = MsoArrowheadStyle.Arrow;
            line.BeginArrowWidth = MsoArrowheadWidth.Wide;
            line.EndType = MsoArrowheadStyle.Arrow;
            line.EndArrowWidth = MsoArrowheadWidth.Narrow;

            // Skriv ut pilspetsstilar och -bredder
            Console.WriteLine("Begin Arrowhead Width: " + line.BeginArrowWidth);
            Console.WriteLine("End Arrowhead Width: " + line.EndArrowWidth);

            // Spara arbetsboken
            workbook.Save("MsoArrowheadWidthExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


