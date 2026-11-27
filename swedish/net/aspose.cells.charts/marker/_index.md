---
title: "Klass Marker"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.Marker class. Representerar markören i ett linjediagram, spridningsdiagram eller radardiagram"
type: docs
url: /sv/net/aspose.cells.charts/marker/
---
## Marker class

Representerar markören i ett linjediagram, spridningsdiagram eller radardiagram.

```csharp
public class Marker
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Area](../../aspose.cells.charts/marker/area/) { get; } | Hämtar [`area`](./area/). |
| [BackgroundColor](../../aspose.cells.charts/marker/backgroundcolor/) { get; set; } | Representerar markörens bakgrundsfärg i ett linjediagram, spridningsdiagram eller radardiagram. |
| [BackgroundColorSetType](../../aspose.cells.charts/marker/backgroundcolorsettype/) { get; set; } | Hämtar eller anger markörens bakgrundsfärgtyp. |
| [Border](../../aspose.cells.charts/marker/border/) { get; } | Hämtar [`border`](../../aspose.cells.drawing/line/). |
| [ForegroundColor](../../aspose.cells.charts/marker/foregroundcolor/) { get; set; } | Representerar markörens förgrundsfärg i ett linjediagram, spridningsdiagram eller radardiagram. |
| [ForegroundColorSetType](../../aspose.cells.charts/marker/foregroundcolorsettype/) { get; set; } | Hämtar eller anger markörens förgrundsfärgtyp. |
| [MarkerSize](../../aspose.cells.charts/marker/markersize/) { get; set; } | Representerar markörens storlek i enheter av punkter. Gäller för linjediagram, spridningsdiagram eller radardiagram. |
| [MarkerSizePx](../../aspose.cells.charts/marker/markersizepx/) { get; set; } | Representerar markörens storlek i enheter av pixlar. Gäller för linjediagram, spridningsdiagram eller radardiagram. |
| [MarkerStyle](../../aspose.cells.charts/marker/markerstyle/) { get; set; } | Representerar markörstilen. Gäller för ett linjediagram, ett spridningsdiagram eller ett radardiagram. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MarkerDemo
    {
        public static void MarkerExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            // Hämta referensen till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till NSeries (diagramdatakälla) till diagrammet som sträcker sig från cellen "A1" till "B3"
            chart.NSeries.Add("A1:B3", true);

            // Åtkomst till den första serien
            Series series = chart.NSeries[0];

            // Ställ in markörens egenskaper
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.MarkerSize = 10; // Size in points
            series.Marker.MarkerSizePx = 20; // Size in pixels
            series.Marker.ForegroundColor = Color.Red;
            series.Marker.ForegroundColorSetType = FormattingType.Custom;
            series.Marker.BackgroundColor = Color.Yellow;
            series.Marker.BackgroundColorSetType = FormattingType.Custom;

            // Spara arbetsboken
            workbook.Save("MarkerExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


