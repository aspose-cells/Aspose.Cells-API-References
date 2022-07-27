---
title: Line
second_title: Aspose.Cells für .NET-API-Referenz
description: Kapselt das Objekt das das Linienformat darstellt.
type: docs
weight: 2200
url: /de/net/aspose.cells.drawing/line/
---
## Line class

Kapselt das Objekt, das das Linienformat darstellt.

```csharp
public class Line
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | Gibt die Länge der Pfeilspitze für den Beginn einer Linie an. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | Gibt die Breite der Pfeilspitze für den Beginn einer Linie an. |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | Gibt eine Pfeilspitze für den Beginn einer Linie an. |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | Gibt die Endbuchstaben an. |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | steht für dieColor der Linie. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | Gibt den Verbundlinientyp an |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | Gibt den Strichlinientyp an |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | Gibt die Länge der Pfeilspitze für das Ende einer Linie an. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | Gibt die Breite der Pfeilspitze für das Ende einer Linie an. |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | Gibt eine Pfeilspitze für das Ende einer Linie an. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | Ruft den Formattyp ab oder legt ihn fest. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | Stellt eine Farbverlaufsfüllung dar. |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | Gibt an, ob dieser Linienstil automatisch zugewiesen wird. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | Gibt an, ob die Linienfarbe automatisch zugewiesen wird. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | Gibt an, ob die Linie sichtbar ist. |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | Gibt die Verbindungskappen an. |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | Repräsentiert den Linienstil. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | Ruft die Designfarbe ab und legt sie fest. |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | Gibt den Transparenzgrad der Linie als Wert von 0,0 (deckend) bis 1,0 (klar) zurück oder legt ihn fest. |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | Ruft ab oder setzt die[`WeightType`](../weighttype) der Linie. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | Holt oder setzt die Gewichtung der Linie in Punkteinheiten. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | Ruft die Linienstärke in Pixeleinheiten ab oder legt sie fest. |

### Beispiele

```csharp

[C#]

Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];

Cells cells = sheet.Cells;
cells[0,1].PutValue("Income");
cells[1,0].PutValue("Company A");
cells[2,0].PutValue("Company B");
cells[3,0].PutValue("Company C");
cells[1,1].PutValue(10000);
cells[2,1].PutValue(20000);
cells[3,1].PutValue(30000);

int chartIndex = sheet.Charts.Add(ChartType.Line, 9, 9, 21, 15);
Chart chart = sheet.Charts[chartIndex];
//Anwenden eines gepunkteten Linienstils auf die Linien eines NSeries
chart.NSeries[0].Border.Style = LineType.Dot;
chart.NSeries[0].Border.Color = Color.Red;
//Anwenden eines dreieckigen Markierungsstils auf die Datenmarkierungen einer NSeries
chart.NSeries[0].Marker.MarkerStyle = ChartMarkerType.Triangle;
//Die Gewichtung aller Zeilen in einer NSeries auf mittel setzen
chart.NSeries[0].Border.Weight = WeightType.MediumLine;

[Visual Basic]

Dim workbook as Workbook = new Workbook()
Dim sheet as Worksheet = workbook.Worksheets(0)

Dim cells as Cells = sheet.Cells
cells(0,1).PutValue("Income")
cells(1,0).PutValue("Company A")
cells(2,0).PutValue("Company B")
cells(3,0).PutValue("Company C")
cells(1,1).PutValue(10000)
cells(2,1).PutValue(20000)
cells(3,1).PutValue(30000)
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)    ///
Dim chart as Chart = sheet.Charts(chartIndex)
'Anwenden eines gepunkteten Linienstils auf die Linien eines NSeries
chart.NSeries(0).Border.Style = LineType.Dot
chart.NSeries(0).Border.Color = Color.Red
'Anwenden eines dreieckigen Markierungsstils auf die Datenmarkierungen eines NSeries
chart.NSeries(0).Marker.MarkerStyle = ChartMarkerType.Triangle
'Einstellen der Gewichtung aller Linien in einer NSeries auf mittel
chart.NSeries(0).Border.Weight = WeightType.MediumLine
```

### Siehe auch

* namensraum [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
