---
title: "Enum MsoLineDashStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.MsoLineDashStyle enum. Representerar stil för streckade ritningslinjer"
type: docs
url: /sv/net/aspose.cells.drawing/msolinedashstyle/
---
## MsoLineDashStyle enumeration

Representerar stil för streckade ritlinjer.

```csharp
public enum MsoLineDashStyle
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Dash | `0` | Representerar en streckad linje. |
| DashDot | `1` | Representerar en streck-punktlinje. |
| DashDotDot | `2` | Representerar en streck-punkt-punktlinje. |
| DashLongDash | `3` | Representerar en linje med långt streck och kort streck. |
| DashLongDashDot | `4` | Representerar en linje med långt streck, kort streck och punkt. |
| RoundDot | `5` | Representerar en linje med runda punkter. |
| Solid | `6` | Representera en solid linje. |
| SquareDot | `7` | Representerar en linje med fyrkantiga punkter. |
| Custom | `8` | Anpassad streckstil. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineDashStyleDemo
    {
        public static void MsoLineDashStyleExample()
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

            // Ställ in streckstilen för de stora rutnätslinjerna
            categoryAxis.MajorGridLines.DashType = MsoLineDashStyle.DashDot;

            // Ställ in streckstilen för de små rutnätslinjerna
            categoryAxis.MinorGridLines.DashType = MsoLineDashStyle.DashLongDashDot;

            // Spara arbetsboken
            workbook.Save("MsoLineDashStyleExample.xlsx");

            // Skriv ut resultaten
            Console.WriteLine("Chart with custom dash styles for gridlines created successfully.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


