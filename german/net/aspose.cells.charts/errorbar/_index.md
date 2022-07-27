---
title: ErrorBar
second_title: Aspose.Cells für .NET-API-Referenz
description: Repräsentiert den Fehlerbalken der Datenreihe.
type: docs
weight: 630
url: /de/net/aspose.cells.charts/errorbar/
---
## ErrorBar class

Repräsentiert den Fehlerbalken der Datenreihe.

```csharp
public class ErrorBar : Line
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Amount](../../aspose.cells.charts/errorbar/amount) { get; set; } | Repräsentiert die Höhe des Fehlerbalkens.  Der Betrag muss größer oder gleich Null sein. |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | Gibt die Länge der Pfeilspitze für den Beginn einer Linie an. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | Gibt die Breite der Pfeilspitze für den Beginn einer Linie an. |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | Gibt eine Pfeilspitze für den Beginn einer Linie an. |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | Gibt die Endbuchstaben an. |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | steht für dieColor der Linie. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | Gibt den Verbundlinientyp an |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | Gibt den Strichlinientyp an |
| [DisplayType](../../aspose.cells.charts/errorbar/displaytype) { get; set; } | Stellt den Anzeigetyp der Fehlerleiste dar. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | Gibt die Länge der Pfeilspitze für das Ende einer Linie an. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | Gibt die Breite der Pfeilspitze für das Ende einer Linie an. |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | Gibt eine Pfeilspitze für das Ende einer Linie an. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | Ruft den Formattyp ab oder legt ihn fest. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | Stellt eine Farbverlaufsfüllung dar. |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | Gibt an, ob dieser Linienstil automatisch zugewiesen wird. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | Gibt an, ob die Linienfarbe automatisch zugewiesen wird. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | Gibt an, ob die Linie sichtbar ist. |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | Gibt die Verbindungskappen an. |
| [MinusValue](../../aspose.cells.charts/errorbar/minusvalue) { get; set; } | Stellt einen negativen Fehlerbetrag dar, wenn der Fehlerbalkentyp Benutzerdefiniert ist. |
| [PlusValue](../../aspose.cells.charts/errorbar/plusvalue) { get; set; } | Stellt einen positiven Fehlerbetrag dar, wenn der Fehlerbalkentyp Benutzerdefiniert ist. |
| [ShowMarkerTTop](../../aspose.cells.charts/errorbar/showmarkerttop) { get; set; } | Gibt an, ob Fehlerbalken mit einem T-Top formatiert werden. |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | Repräsentiert den Linienstil. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | Ruft die Designfarbe ab und legt sie fest. |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | Gibt den Transparenzgrad der Linie als Wert von 0,0 (deckend) bis 1,0 (klar) zurück oder legt ihn fest. |
| [Type](../../aspose.cells.charts/errorbar/type) { get; set; } | Repräsentiert den Betragstyp des Fehlerbalkens. |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | Ruft ab oder setzt die[`WeightType`](../../aspose.cells.drawing/weighttype) der Linie. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | Holt oder setzt die Gewichtung der Linie in Punkteinheiten. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | Ruft die Linienstärke in Pixeleinheiten ab oder legt sie fest. |

### Beispiele

```csharp
[C#]
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["a1"].PutValue(2);
cells["a2"].PutValue(5);
cells["a3"].PutValue(3);
cells["a4"].PutValue(6);
cells["b1"].PutValue(4);
cells["b2"].PutValue(3);
cells["b3"].PutValue(6);
cells["b4"].PutValue(7);

cells["C1"].PutValue("Q1");
cells["C2"].PutValue("Q2");
cells["C3"].PutValue("Y1");
cells["C4"].PutValue("Y2");

int chartIndex = excel.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);

Chart chart = excel.Worksheets[0].Charts[chartIndex];
chart.NSeries.Add("A1:B4", true);

chart.NSeries.CategoryData = "C1:C4";

for(int i = 0; i < chart.NSeries.Count; i ++)
{
	ASeries aseries = chart.NSeries[i];
	aseries.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
	aseries.YErrorBar.Type = ErrorBarType.FixedValue;
	aseries.YErrorBar.Amount = 5;
}

[Visual Basic]
Dim workbook As Workbook =  New Workbook() 
Dim cells As Cells =  workbook.Worksheets(0).Cells 
cells("a1").PutValue(2)
cells("a2").PutValue(5)
cells("a3").PutValue(3)
cells("a4").PutValue(6)
cells("b1").PutValue(4)
cells("b2").PutValue(3)
cells("b3").PutValue(6)
cells("b4").PutValue(7)

cells("C1").PutValue("Q1")
cells("C2").PutValue("Q2")
cells("C3").PutValue("Y1")
cells("C4").PutValue("Y2")

Dim chartIndex As Integer =  excel.Worksheets(0).Charts.Add(ChartType.Column,11,0,27,10) 

Dim chart As Chart =  excel.Worksheets(0).Charts(chartIndex) 
chart.NSeries.Add("A1:B4", True)

chart.NSeries.CategoryData = "C1:C4"

Dim i As Integer
For  i = 0 To chart.NSeries.Count - 1
Dim aseries As ASeries =  chart.NSeries(i) 
aseries.YErrorBar.DisplayType = ErrorBarDisplayType.Minus
aseries.YErrorBar.Type = ErrorBarType.FixedValue
aseries.YErrorBar.Amount = 5
Next
```

### Siehe auch

* class [Line](../../aspose.cells.drawing/line)
* namensraum [Aspose.Cells.Charts](../../aspose.cells.charts)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
