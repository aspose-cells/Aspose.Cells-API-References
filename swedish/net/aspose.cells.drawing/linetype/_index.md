---
title: "Enum LineType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.LineType enum. Enumererar typen av Picture-kant eller Chart-linje."
type: docs
url: /sv/net/aspose.cells.drawing/linetype/
---
## LineType enumeration

Enumererar typen av [`Picture`](../picture/) kant eller [`Chart`](../../aspose.cells.charts/chart/) linje.

```csharp
public enum LineType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| DarkGray | `6` | Representerar en mörkgrå linje. |
| Dash | `1` | Representerar en streckad linje. |
| DashDot | `3` | Representerar en streck-punktlinje |
| DashDotDot | `4` | Representerar en streck-punkt-punktlinje. |
| Dot | `2` | Representerar en prickad linje. |
| LightGray | `8` | Representerar en ljusgrå linje. |
| MediumGray | `7` | Representerar en medelgrå linje. |
| Solid | `0` | Representera en solid linje. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class LineTypeDemo
    {
        public static void LineTypeExample()
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

            // Ställ in linjetypen för axellinjen
            categoryAxis.AxisLine.Style = LineType.DashDot;

            // Ställ in färgen på axellinjen
            categoryAxis.AxisLine.Color = Color.Blue;

            // Åtkomst till den primära värdeaxeln
            Axis valueAxis = chart.ValueAxis;

            // Ställ in linjetypen för huvudrutnätslinjerna
            valueAxis.MajorGridLines.Style = LineType.Dot;

            // Ställ in färgen på huvudrutnätslinjerna
            valueAxis.MajorGridLines.Color = Color.Red;

            // Spara arbetsboken
            workbook.Save("LineTypeExample.xlsx");

            // Skriv ut resultaten
            Console.WriteLine("Chart created with custom line types for axis and gridlines.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


