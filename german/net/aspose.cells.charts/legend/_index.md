---
title: Legend
second_title: Aspose.Cells für .NET-API-Referenz
description: Kapselt das Objekt das die Diagrammlegende darstellt.
type: docs
weight: 690
url: /de/net/aspose.cells.charts/legend/
---
## Legend class

Kapselt das Objekt, das die Diagrammlegende darstellt.

```csharp
public class Legend : ChartTextFrame
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | Ruft die ab[`Bereich`](../chartframe/area) . |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont) { get; set; } | True, wenn der Text im Objekt die Schriftgröße ändert, wenn sich die Objektgröße ändert. Der Standardwert ist True. |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | Liest und setzt den Anzeigemodus des Hintergrunds |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | Ruft die ab[`Grenze`](../../aspose.cells.drawing/line) . |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Stellt die Höhe der Standardposition dar |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Repräsentiert die Breite der Standardposition |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Stellt x der Standardposition dar |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Stellt y der Standardposition dar |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype) { get; set; } | Ruft die Textrichtung ab und legt sie fest. |
| virtual [Font](../../aspose.cells.charts/chartframe/font) { get; } | erhält a[`Font`](../chartframe/font) Objekt des angegebenen ChartFrame-Objekts. |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | Ruft die Rahmenhöhe in Einheiten von 1/4000 des Diagrammbereichs ab oder legt sie fest. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Gibt an, ob die Größe des Diagrammrahmens automatisch angepasst wird. |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext) { get; set; } | Gibt an, dass der Text automatisch generiert wird. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Gibt an, ob die Standardposition (DefaultX, DefaultY, DefaultWidth und DefaultHeight) eingestellt ist. |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | Gibt an, ob diese Datenbeschriftung gelöscht wurde. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Gibt an, ob die Größe des Plotbereichs die Teilstriche und die Achsenbeschriftungen umfasst. False gibt an, dass die Größe die Größe des Plotbereichs, der Teilstriche und der Achsenbeschriftungen bestimmen soll. |
| [IsOverLay](../../aspose.cells.charts/legend/isoverlay) { get; set; } | Ermittelt oder setzt, ob andere Diagrammelemente dieses Diagrammelement überlappen dürfen. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Ruft ab oder legt fest, ob eine Form automatisch angepasst werden soll, um den darin beschriebenen Text vollständig zu enthalten. Die automatische Anpassung ist , wenn Text innerhalb einer Form skaliert wird, um den gesamten darin enthaltenen Text aufzunehmen. |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Text umbrochen wird. |
| [LegendEntries](../../aspose.cells.charts/legend/legendentries) { get; } | Ruft eine Sammlung aller LegendEntry-Objekte in der angegebenen Diagrammlegende ab. Das Festlegen der Legendeneinträge des Oberflächendiagramms wird nicht unterstützt. Daher wird null zurückgegeben, wenn der Diagrammtyp ein Oberflächendiagrammtyp ist. |
| [LegendEntriesLabels](../../aspose.cells.charts/legend/legendentrieslabels) { get; } | Ruft die Beschriftungen der Legendeneinträge nach dem Aufruf der Methode Chart.Calculate() ab. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Ruft einen Verweis auf das Arbeitsblatt ab und legt ihn fest. |
| [Position](../../aspose.cells.charts/legend/position) { get; set; } | Ruft den Positionstyp der Legende ab oder legt ihn fest. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Stellt die Lesereihenfolge des Textes dar. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Stellt den Drehwinkel des Textes dar. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | True, wenn der Rahmen einen Schatten hat. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Ruft die ab[`ShapeProperties`](../chartframe/shapeproperties) Objekt. |
| virtual [Text](../../aspose.cells.charts/charttextframe/text) { get; set; } | Ruft den Text des Titels eines Frames ab oder legt ihn fest. |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment) { get; set; } | Ruft die horizontale Textausrichtung ab und legt sie fest. |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment) { get; set; } | Ruft die vertikale Textausrichtung von Text ab oder legt sie fest. |
| virtual [Width](../../aspose.cells.charts/chartframe/width) { get; set; } | Ruft die Rahmenbreite in Einheiten von 1/4000 des Diagrammbereichs ab oder legt sie fest. |
| virtual [X](../../aspose.cells.charts/chartframe/x) { get; set; } | Ruft die x-Koordinate der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs ab oder legt sie fest. |
| virtual [Y](../../aspose.cells.charts/chartframe/y) { get; set; } | Liest oder setzt die y-Koordinate der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Characters](../../aspose.cells.charts/charttextframe/characters)(int, int) | Gibt ein Characters-Objekt zurück, das einen Bereich von Zeichen im Text darstellt. |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Position des Rahmens auf automatisch setzen |

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
		
int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
Chart chart = sheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
//Breite und Höhe der Legende festlegen
Legend legend = chart.Legend;

//Legende befindet sich standardmäßig auf der rechten Seite des Diagramms.
//Wenn sich die Legende auf der linken oder rechten Seite des Diagramms befindet, wird die Einstellung der Legend.X-Eigenschaft nicht wirksam.
//Wenn sich die Legende an der oberen oder unteren Seite des Diagramms befindet, wird die Einstellung der Legend.Y-Eigenschaft nicht wirksam.
legend.Y = 1500;
legend.Width = 50;
legend.Height = 50; 
// Legen Sie die Position der Legende fest
legend.Position = LegendPositionType.Left;

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
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)

Dim chart as Chart = sheet.Charts(chartIndex)
chart.SetChartDataRange("A1:B4", True);
 
'Set Legend's width and height
Dim legend as Legend = chart.Legend

'Die Legende befindet sich standardmäßig auf der rechten Seite des Diagramms.
'Wenn sich die Legende auf der linken oder rechten Seite des Diagramms befindet, wird die Einstellung der Legend.X-Eigenschaft nicht wirksam.
'Wenn sich die Legende an der oberen oder unteren Seite des Diagramms befindet, wird die Einstellung der Legend.Y-Eigenschaft nicht wirksam.
legend.Y = 1500
legend.Width = 50
legend.Height = 50
'Set legend's position
legend.Position = LegendPositionType.Left
```

### Siehe auch

* class [ChartTextFrame](../charttextframe)
* namensraum [Aspose.Cells.Charts](../../aspose.cells.charts)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
