---
title: "Klass Area"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Area klass. Inkapslar objektet som representerar ett områdesformat"
type: docs
url: /sv/net/aspose.cells.drawing/area/
---
## Area class

Inkapslar objektet som representerar ett områdesformat.

```csharp
public class Area
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Hämtar eller anger bakgrundsfärgen för `Area`. |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Representerar ett [`FillFormat`](./fillformat/)‑objekt som innehåller fyllningsformaterings‑egenskaper för det angivna diagrammet eller formen. |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Hämtar eller anger förgrundsfärgen. |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Representerar formateringen av området. |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | Om egenskapen är sann och värdet för diagrampunkten är ett negativt tal, kommer förgrundsfärgen och bakgrundsfärgen att bytas ut. |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Returnerar eller anger graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (klar). |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class AreaDemo
    {
        public static void AreaExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            // Lägga till ett nytt kalkylblad i Workbook-objektet
            int sheetIndex = workbook.Worksheets.Add();
            // Hämtar referensen till det nyligen tillagda kalkylbladet genom att ange dess bladindex
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Lägger till exempelvärden i celler
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(-100);
            worksheet.Cells["A3"].PutValue(150);
            // Lägger till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 15, 5);
            // Åtkomst till instansen av det nyligen tillagda diagrammet
            Chart chart = worksheet.Charts[chartIndex];
            // Lägger till NSeries (diagramdatakälla) till diagrammet från cellen "A1" till "A3"
            chart.NSeries.Add("A1:A3", true);

            // Åtkomst till området för den första NSeries
            Area area = chart.NSeries[0].Area;

            // Ställa in egenskaper
            area.InvertIfNegative = true;
            area.ForegroundColor = Color.Red;
            area.BackgroundColor = Color.Yellow;
            area.Formatting = Aspose.Cells.Charts.FormattingType.Custom;
            area.Transparency = 0.5;

            // Sparar Excel-filen
            workbook.Save("AreaExample.xlsx");
            workbook.Save("AreaExample.pdf");

        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


