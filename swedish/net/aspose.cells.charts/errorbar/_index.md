---
title: "Klass ErrorBar"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.ErrorBar-klass. Representerar felstapeln för dataserier"
type: docs
url: /sv/net/aspose.cells.charts/errorbar/
---
## ErrorBar class

Representerar felstapeln för dataserien.

```csharp
public class ErrorBar : Line
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Amount](../../aspose.cells.charts/errorbar/amount/) { get; set; } | Representerar mängden felstapel. |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength/) { get; set; } | Anger längden på pilspetsen för början av en linje.(Ärvd från [`Line`](../../aspose.cells.drawing/line/).) |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth/) { get; set; } | Anger bredden på pilspetsen för början av en linje.(Ärvd från [`Line`](../../aspose.cells.drawing/line/).) |
| [BeginType](../../aspose.cells.drawing/line/begintype/) { get; set; } | Anger en pilspets för början av en linje.(Ärvd från [`Line`](../../aspose.cells.drawing/line/).) |
| [CapType](../../aspose.cells.drawing/line/captype/) { get; set; } | Anger avslutningskapparna.(Ärvt från [`Line`](../../aspose.cells.drawing/line/).) |
| [Color](../../aspose.cells.drawing/line/color/) { get; set; } | Representerar färgen på linjen.(Ärvt från [`Line`](../../aspose.cells.drawing/line/).) |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype/) { get; set; } | Anger den sammansatta linjetypen(Ärvt från [`Line`](../../aspose.cells.drawing/line/).) |
| [DashType](../../aspose.cells.drawing/line/dashtype/) { get; set; } | Anger strecklinjetypen(Ärvt från [`Line`](../../aspose.cells.drawing/line/).) |
| [DisplayType](../../aspose.cells.charts/errorbar/displaytype/) { get; set; } | Representerar visningstypen för felstapeln. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength/) { get; set; } | Anger längden på pilspetsen för slutet av en linje.(Ärvt från [`Line`](../../aspose.cells.drawing/line/).) |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth/) { get; set; } | Anger bredden på pilspetsen för slutet av en linje.(Ärvt från [`Line`](../../aspose.cells.drawing/line/).) |
| [EndType](../../aspose.cells.drawing/line/endtype/) { get; set; } | Anger en pilspets för slutet av en linje.(Ärvt från [`Line`](../../aspose.cells.drawing/line/).) |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype/) { get; set; } | Hämtar eller anger formattyp.(Ärvt från [`Line`](../../aspose.cells.drawing/line/).) |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill/) { get; } | Representerar gradientfyllning.(Ärvt från [`Line`](../../aspose.cells.drawing/line/).) |
| [IsAuto](../../aspose.cells.drawing/line/isauto/) { get; set; } | Indikerar om denna linjestil tilldelas automatiskt.(Ärvt från [`Line`](../../aspose.cells.drawing/line/).) |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor/) { get; } | Indikerar om linjens färg tilldelas automatiskt.(Ärvt från [`Line`](../../aspose.cells.drawing/line/).) |
| [IsVisible](../../aspose.cells.drawing/line/isvisible/) { get; set; } | Representerar om linjen är synlig.(Ärvt från [`Line`](../../aspose.cells.drawing/line/).) |
| [JoinType](../../aspose.cells.drawing/line/jointype/) { get; set; } | Anger anslutningskapparna.(Ärvt från [`Line`](../../aspose.cells.drawing/line/).) |
| [MinusValue](../../aspose.cells.charts/errorbar/minusvalue/) { get; set; } | Representerar negativt felvärde när felstapeln är av typen Custom. |
| [PlusValue](../../aspose.cells.charts/errorbar/plusvalue/) { get; set; } | Representerar positivt felvärde när felstapeln är Custom. |
| [ShowMarkerTTop](../../aspose.cells.charts/errorbar/showmarkerttop/) { get; set; } | Indikerar om felstaplar formateras med en T-top. |
| [Style](../../aspose.cells.drawing/line/style/) { get; set; } | Representerar linjens stil.(Ärvt från [`Line`](../../aspose.cells.drawing/line/).) |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor/) { get; set; } | Hämtar och anger temafärgen.(Ärvt från [`Line`](../../aspose.cells.drawing/line/).) |
| [Transparency](../../aspose.cells.drawing/line/transparency/) { get; set; } | Returnerar eller anger graden av transparens för linjen som ett värde från 0.0 (opak) till 1.0 (klar).(ärvd från [`Line`](../../aspose.cells.drawing/line/).) |
| [Type](../../aspose.cells.charts/errorbar/type/) { get; set; } | Representerar felstapels mängdtyp. |
| [Weight](../../aspose.cells.drawing/line/weight/) { get; set; } | Hämtar eller anger [`WeightType`](../../aspose.cells.drawing/weighttype/) för linjen.(ärvd från [`Line`](../../aspose.cells.drawing/line/).) |
| [WeightPt](../../aspose.cells.drawing/line/weightpt/) { get; set; } | Hämtar eller anger vikten på linjen i enheter av punkter.(ärvd från [`Line`](../../aspose.cells.drawing/line/).) |
| [WeightPx](../../aspose.cells.drawing/line/weightpx/) { get; set; } | Hämtar eller anger vikten på linjen i enheter av pixlar.(ärvd från [`Line`](../../aspose.cells.drawing/line/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ErrorBarDemo
    {
        public static void ErrorBarExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Lägg till exempeldata i celler
            cells["A1"].PutValue(2);
            cells["A2"].PutValue(5);
            cells["A3"].PutValue(3);
            cells["A4"].PutValue(6);
            cells["B1"].PutValue(4);
            cells["B2"].PutValue(3);
            cells["B3"].PutValue(6);
            cells["B4"].PutValue(7);
            cells["C1"].PutValue("Q1");
            cells["C2"].PutValue("Q2");
            cells["C3"].PutValue("Y1");
            cells["C4"].PutValue("Y2");

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];

            // Lägg till NSeries (diagramdatakälla) till diagrammet
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Konfigurera felstaplar för varje serie i diagrammet
            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                Series series = chart.NSeries[i];
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5;

                // Ytterligare egenskaper för demonstration
                series.YErrorBar.ShowMarkerTTop = true;
                series.YErrorBar.PlusValue = "=Sheet1!A1";
                series.YErrorBar.MinusValue = "=Sheet1!A2";
                series.YErrorBar.CompoundType = Aspose.Cells.Drawing.MsoLineStyle.ThickThin;
                series.YErrorBar.DashType = Aspose.Cells.Drawing.MsoLineDashStyle.DashDot;
                series.YErrorBar.CapType = Aspose.Cells.Drawing.LineCapType.Round;
                series.YErrorBar.JoinType = Aspose.Cells.Drawing.LineJoinType.Bevel;
                series.YErrorBar.BeginType = Aspose.Cells.Drawing.MsoArrowheadStyle.Arrow;
                series.YErrorBar.EndType = Aspose.Cells.Drawing.MsoArrowheadStyle.ArrowDiamond;
                series.YErrorBar.BeginArrowLength = Aspose.Cells.Drawing.MsoArrowheadLength.Short;
                series.YErrorBar.EndArrowLength = Aspose.Cells.Drawing.MsoArrowheadLength.Long;
                series.YErrorBar.BeginArrowWidth = Aspose.Cells.Drawing.MsoArrowheadWidth.Narrow;
                series.YErrorBar.EndArrowWidth = Aspose.Cells.Drawing.MsoArrowheadWidth.Wide;
                series.YErrorBar.ThemeColor = new Aspose.Cells.ThemeColor(Aspose.Cells.ThemeColorType.Accent1, 0.5);
                series.YErrorBar.Color = System.Drawing.Color.Red;
                series.YErrorBar.Transparency = 0.5;
                series.YErrorBar.Style = Aspose.Cells.Drawing.LineType.DashDotDot;
                series.YErrorBar.Weight = Aspose.Cells.Drawing.WeightType.WideLine;
                series.YErrorBar.WeightPt = 2.0;
                series.YErrorBar.WeightPx = 3.0;
                series.YErrorBar.FormattingType = ChartLineFormattingType.Gradient;
                series.YErrorBar.IsVisible = true;
                series.YErrorBar.IsAuto = false;
            }

            // Spara arbetsboken
            workbook.Save("ErrorBarExample.xlsx");
            workbook.Save("ErrorBarExample.pdf");
        }
    }
}
```

### Se även

* class [Line](../../aspose.cells.drawing/line/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


