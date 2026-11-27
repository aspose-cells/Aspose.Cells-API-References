---
title: "Enum MsoLineStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.MsoLineStyle-enum. Representerar stil för ritade linjer"
type: docs
url: /sv/net/aspose.cells.drawing/msolinestyle/
---
## MsoLineStyle enumeration

Representerar stil för ritlinjer.

```csharp
public enum MsoLineStyle
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Single | `0` | Enkel linje (med bredd lineWidth) |
| ThickBetweenThin | `1` | Tre linjer, tunn, tjock, tunn |
| ThinThick | `2` | Dubbla linjer, en tunn, en tjock |
| ThickThin | `3` | Dubbla linjer, en tjock, en tunn |
| ThinThin | `4` | Dubbla linjer med lika bredd |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineStyleDemo
    {
        public static void MsoLineStyleExample()
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

            // Åtkomst till den primära kategoraxeln
            Axis categoryAxis = chart.CategoryAxis;

            // Ställ in linjestilen för den primära kategoraxeln
            Line axisLine = categoryAxis.AxisLine;
            axisLine.CompoundType = MsoLineStyle.ThickBetweenThin;
            axisLine.Color = Color.Blue;
            axisLine.WeightPt = 2.0;

            // Skriv ut linjestilen
            Console.WriteLine("Axis Line Style: " + axisLine.CompoundType);
            Console.WriteLine("Axis Line Color: " + axisLine.Color);
            Console.WriteLine("Axis Line Weight: " + axisLine.WeightPt);

            // Spara arbetsboken
            workbook.Save("MsoLineStyleExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


