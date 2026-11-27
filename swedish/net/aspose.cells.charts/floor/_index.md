---
title: "Klass Floor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.Floor klass. Inkapslar objektet som representerar golvet i ett 3D-diagram"
type: docs
url: /sv/net/aspose.cells.charts/floor/
---
## Floor class

Inkapslar objektet som representerar golvet i ett 3‑D‑diagram.

```csharp
public class Floor : Area
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Hämtar eller anger bakgrundsfärgen för [`Area`](../../aspose.cells.drawing/area/).(Ärvd från [`Area`](../../aspose.cells.drawing/area/).) |
| [Border](../../aspose.cells.charts/floor/border/) { get; set; } | Hämtar eller anger kantens [`Line`](../../aspose.cells.drawing/line/). |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Representerar ett [`FillFormat`](../../aspose.cells.drawing/area/fillformat/)‑objekt som innehåller fyllningsformaterings‑egenskaper för det angivna diagrammet eller formen.(Ärvd från [`Area`](../../aspose.cells.drawing/area/).) |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Hämtar eller anger förgrundsfärgen.(Ärvd från [`Area`](../../aspose.cells.drawing/area/).) |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Representerar formateringen av området.(Ärvd från [`Area`](../../aspose.cells.drawing/area/).) |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | Om egenskapen är sann och värdet för diagrampunkten är ett negativt tal, kommer förgrundsfärgen och bakgrundsfärgen att bytas ut.(Ärvd från [`Area`](../../aspose.cells.drawing/area/).) |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Returnerar eller anger graden av transparens för området som ett värde från 0.0 (opak) genom 1.0 (klar).(Ärvd från [`Area`](../../aspose.cells.drawing/area/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FloorDemo
    {
        public static void FloorExample()
        {
            // Instansiera arbetsbokobjektet
            Workbook workbook = new Workbook();

            // Hämta cellsamling
            Cells cells = workbook.Worksheets[0].Cells;

            // Sätt värden i celler
            cells["A1"].PutValue(1);
            cells["A2"].PutValue(2);
            cells["A3"].PutValue(3);

            // Hämta diagramsamling
            ChartCollection charts = workbook.Worksheets[0].Charts;

            // Lägg till ett nytt diagram
            int index = charts.Add(ChartType.Column3DStacked, 5, 0, 15, 5);

            // Hämta det nyligen tillagda diagrammet
            Chart chart = charts[index];

            // Ställ in diagrammets nseries
            chart.NSeries.Add("A1:A3", true);

            // Visa dataetiketter
            chart.NSeries[0].DataLabels.ShowValue = true;

            // Hämta diagrammets golv
            Floor floor = chart.Floor;

            // Ställ in golvets kant som röd
            floor.Border.Color = Color.Red;

            // Ställ in fyllningsformat
            floor.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.DiagonalDown, 2);

            // Ange ytterligare egenskaper
            floor.BackgroundColor = Color.LightBlue;
            floor.ForegroundColor = Color.DarkBlue;
            floor.Formatting = FormattingType.Custom;
            floor.InvertIfNegative = true;
            floor.Transparency = 0.5;

            // Spara filen
            workbook.Save(@"FloorExample.xlsx");
            workbook.Save(@"FloorExample.pdf");
        }
    }
}
```

### Se även

* class [Area](../../aspose.cells.drawing/area/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


