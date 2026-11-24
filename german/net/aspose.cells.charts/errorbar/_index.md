---
title: "Klasse ErrorBar"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.ErrorBar Klasse. Stellt die Fehlermarge einer Datenreihe dar"
type: docs
url: /de/net/aspose.cells.charts/errorbar/
---
## ErrorBar class

Stellt den Fehlerbalken einer Datenserie dar.

```csharp
public class ErrorBar : Line
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Amount](../../aspose.cells.charts/errorbar/amount/) { get; set; } | Stellt die Größe der Fehlermarge dar. |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength/) { get; set; } | Gibt die Länge der Pfeilspitze für den Anfang einer Linie an.(Vererbt von [`Line`](../../aspose.cells.drawing/line/).) |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth/) { get; set; } | Gibt die Breite der Pfeilspitze für den Anfang einer Linie an.(Vererbt von [`Line`](../../aspose.cells.drawing/line/).) |
| [BeginType](../../aspose.cells.drawing/line/begintype/) { get; set; } | Gibt eine Pfeilspitze für den Anfang einer Linie an.(Vererbt von [`Line`](../../aspose.cells.drawing/line/).) |
| [CapType](../../aspose.cells.drawing/line/captype/) { get; set; } | Gibt die Endkappen an.(Vererbt von [`Line`](../../aspose.cells.drawing/line/).) |
| [Color](../../aspose.cells.drawing/line/color/) { get; set; } | Stellt die Farbe der Linie dar.(Vererbt von [`Line`](../../aspose.cells.drawing/line/).) |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype/) { get; set; } | Gibt den zusammengesetzten Linientyp an(Vererbt von [`Line`](../../aspose.cells.drawing/line/).) |
| [DashType](../../aspose.cells.drawing/line/dashtype/) { get; set; } | Gibt den Strichlinientyp an (geerbt von [`Line`](../../aspose.cells.drawing/line/).) |
| [DisplayType](../../aspose.cells.charts/errorbar/displaytype/) { get; set; } | Stellt den Anzeigetyp der Fehlermarge dar. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength/) { get; set; } | Gibt die Länge der Pfeilspitze am Ende einer Linie an (geerbt von [`Line`](../../aspose.cells.drawing/line/).) |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth/) { get; set; } | Gibt die Breite der Pfeilspitze am Ende einer Linie an (geerbt von [`Line`](../../aspose.cells.drawing/line/).) |
| [EndType](../../aspose.cells.drawing/line/endtype/) { get; set; } | Gibt eine Pfeilspitze für das Ende einer Linie an (geerbt von [`Line`](../../aspose.cells.drawing/line/).) |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype/) { get; set; } | Liest oder setzt den Formattyp (geerbt von [`Line`](../../aspose.cells.drawing/line/).) |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill/) { get; } | Stellt einen Farbverlauf dar (geerbt von [`Line`](../../aspose.cells.drawing/line/).) |
| [IsAuto](../../aspose.cells.drawing/line/isauto/) { get; set; } | Gibt an, ob dieser Linienstil automatisch zugewiesen wird (geerbt von [`Line`](../../aspose.cells.drawing/line/).) |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor/) { get; } | Gibt an, ob die Farbe der Linie automatisch zugewiesen wird (geerbt von [`Line`](../../aspose.cells.drawing/line/).) |
| [IsVisible](../../aspose.cells.drawing/line/isvisible/) { get; set; } | Stellt dar, ob die Linie sichtbar ist (geerbt von [`Line`](../../aspose.cells.drawing/line/).) |
| [JoinType](../../aspose.cells.drawing/line/jointype/) { get; set; } | Gibt die Verbindungsenden an (geerbt von [`Line`](../../aspose.cells.drawing/line/).) |
| [MinusValue](../../aspose.cells.charts/errorbar/minusvalue/) { get; set; } | Stellt den negativen Fehlermengenwert dar, wenn der Fehlermargen-Typ benutzerdefiniert ist. |
| [PlusValue](../../aspose.cells.charts/errorbar/plusvalue/) { get; set; } | Stellt den positiven Fehlermengenwert dar, wenn der Fehlermargen-Typ benutzerdefiniert ist. |
| [ShowMarkerTTop](../../aspose.cells.charts/errorbar/showmarkerttop/) { get; set; } | Gibt an, ob Fehlermargen mit einem T-Oben formatiert werden. |
| [Style](../../aspose.cells.drawing/line/style/) { get; set; } | Stellt den Stil der Linie dar (geerbt von [`Line`](../../aspose.cells.drawing/line/).) |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor/) { get; set; } | Liest und setzt die Themenfarbe (geerbt von [`Line`](../../aspose.cells.drawing/line/).) |
| [Transparency](../../aspose.cells.drawing/line/transparency/) { get; set; } | Gibt den Transparenzgrad der Linie zurück oder setzt ihn als Wert von 0,0 (undurchsichtig) bis 1,0 (klar) (geerbt von [`Line`](../../aspose.cells.drawing/line/).) |
| [Type](../../aspose.cells.charts/errorbar/type/) { get; set; } | Stellt den Betragstyp der Fehlermarge dar. |
| [Weight](../../aspose.cells.drawing/line/weight/) { get; set; } | Liest oder setzt den [`WeightType`](../../aspose.cells.drawing/weighttype/) der Linie (geerbt von [`Line`](../../aspose.cells.drawing/line/).) |
| [WeightPt](../../aspose.cells.drawing/line/weightpt/) { get; set; } | Liest oder setzt die Stärke der Linie in Punkten.(Vererbt von [`Line`](../../aspose.cells.drawing/line/).) |
| [WeightPx](../../aspose.cells.drawing/line/weightpx/) { get; set; } | Liest oder setzt die Stärke der Linie in Pixeln.(Vererbt von [`Line`](../../aspose.cells.drawing/line/).) |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Füge Beispieldaten zu Zellen hinzu
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

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];

            // Füge NSeries (Diagrammdatenquelle) zum Diagramm hinzu
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Konfiguriere Fehlermarken für jede Serie im Diagramm
            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                Series series = chart.NSeries[i];
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5;

                // Zusätzliche Eigenschaften zur Demonstration
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

            // Speichere die Arbeitsmappe
            workbook.Save("ErrorBarExample.xlsx");
            workbook.Save("ErrorBarExample.pdf");
        }
    }
}
```

### Siehe auch

* class [Line](../../aspose.cells.drawing/line/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


