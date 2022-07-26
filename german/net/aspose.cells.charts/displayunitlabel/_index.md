---
title: DisplayUnitLabel
second_title: Aspose.Cells für .NET-API-Referenz
description: Repräsentiert das Etikett der Anzeigeeinheit.
type: docs
weight: 600
url: /de/net/aspose.cells.charts/displayunitlabel/
---
## DisplayUnitLabel class

Repräsentiert das Etikett der Anzeigeeinheit.

```csharp
public class DisplayUnitLabel : ChartTextFrame
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | Ruft die ab[`Bereich`](../chartframe/area) . |
| override [AutoScaleFont](../../aspose.cells.charts/displayunitlabel/autoscalefont) { get; set; } | True, wenn der Text im Objekt die Schriftgröße ändert, wenn sich die Objektgröße ändert. Der Standardwert ist True. |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | Liest und setzt den Anzeigemodus des Hintergrunds |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | Ruft die ab[`Grenze`](../../aspose.cells.drawing/line) . |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Stellt die Höhe der Standardposition dar |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Repräsentiert die Breite der Standardposition |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Stellt x der Standardposition dar |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Stellt y der Standardposition dar |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype) { get; set; } | Ruft die Textrichtung ab und legt sie fest. |
| override [Font](../../aspose.cells.charts/displayunitlabel/font) { get; } | erhält a[`Font`](./font) Objekt des angegebenen ChartFrame-Objekts. |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | Ruft die Rahmenhöhe in Einheiten von 1/4000 des Diagrammbereichs ab oder legt sie fest. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Gibt an, ob die Größe des Diagrammrahmens automatisch angepasst wird. |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext) { get; set; } | Gibt an, dass der Text automatisch generiert wird. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Gibt an, ob die Standardposition (DefaultX, DefaultY, DefaultWidth und DefaultHeight) eingestellt ist. |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | Gibt an, ob diese Datenbeschriftung gelöscht wurde. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Gibt an, ob die Größe des Plotbereichs die Teilstriche und die Achsenbeschriftungen umfasst. False gibt an, dass die Größe die Größe des Plotbereichs, der Teilstriche und der Achsenbeschriftungen bestimmen soll. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Ruft ab oder legt fest, ob eine Form automatisch angepasst werden soll, um den darin beschriebenen Text vollständig zu enthalten. Die automatische Anpassung ist , wenn Text innerhalb einer Form skaliert wird, um den gesamten darin enthaltenen Text aufzunehmen. |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Text umbrochen wird. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Ruft einen Verweis auf das Arbeitsblatt ab und legt ihn fest. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Stellt die Lesereihenfolge des Textes dar. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Stellt den Drehwinkel des Textes dar. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | True, wenn der Rahmen einen Schatten hat. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Ruft die ab[`ShapeProperties`](../chartframe/shapeproperties) Objekt. |
| override [Text](../../aspose.cells.charts/displayunitlabel/text) { get; set; } | Ruft den Text der Bezeichnung der Anzeigeeinheit ab oder legt ihn fest. |
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

//Instanziieren eines Workbook-Objekts
Workbook workbook = new Workbook();
//Hinzufügen eines neuen Arbeitsblatts zum Excel-Objekt
int sheetIndex = workbook.Worksheets.Add();
//Beziehen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergeben seines Blattindex
Worksheet worksheet = workbook.Worksheets[sheetIndex];
//Hinzufügen eines Beispielwerts zur Zelle "A1".
worksheet.Cells["A1"].PutValue(50);
//Hinzufügen eines Beispielwerts zur Zelle "A2".
worksheet.Cells["A2"].PutValue(100);
//Hinzufügen eines Beispielwerts zur Zelle "A3".
worksheet.Cells["A3"].PutValue(150);
//Hinzufügen eines Beispielwerts zur Zelle "A4".
worksheet.Cells["A4"].PutValue(200);
//Hinzufügen eines Beispielwerts zur Zelle "B1".
worksheet.Cells["B1"].PutValue(60);
//Hinzufügen eines Beispielwerts zur Zelle "B2".
worksheet.Cells["B2"].PutValue(32);
//Hinzufügen eines Beispielwerts zur Zelle "B3".
worksheet.Cells["B3"].PutValue(50);
//Hinzufügen eines Beispielwerts zur Zelle "B4".
worksheet.Cells["B4"].PutValue(40);
//Hinzufügen eines Beispielwerts zur Zelle "C1" als Kategoriedaten
worksheet.Cells["C1"].PutValue("Q1");
//Hinzufügen eines Beispielwerts zur Zelle "C2" als Kategoriedaten
worksheet.Cells["C2"].PutValue("Q2");
//Hinzufügen eines Beispielwerts zur Zelle "C3" als Kategoriedaten
worksheet.Cells["C3"].PutValue("Y1");
//Hinzufügen eines Beispielwerts zur Zelle "C4" als Kategoriedaten
worksheet.Cells["C4"].PutValue("Y2");
//Hinzufügen eines Diagramms zum Arbeitsblatt
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
//Auf die Instanz des neu hinzugefügten Diagramms zugreifen
Chart chart = worksheet.Charts[chartIndex];
//Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm im Bereich von Zelle "A1" bis "B4"
chart.NSeries.Add("A1:B4", true);
//Festlegen der Datenquelle für die Kategoriedaten von NSeries
chart.NSeries.CategoryData = "C1:C4";
// Einstellen der Anzeigeeinheit der Wertachse (Y).
chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
DisplayUnitLabel displayUnitLabel = chart.ValueAxis.DisplayUnitLabel;
//Festlegen der Beschriftung der benutzerdefinierten Anzeigeeinheit
displayUnitLabel.Text = "100";
//Speichern der Excel-Datei
workbook.Save("book1.xls");

[Visual Basic]

'Instanziieren eines Workbook-Objekts
Dim workbook As Workbook = New Workbook()
'Hinzufügen eines neuen Arbeitsblatts zum Excel-Objekt
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergeben seines Blattindex
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)
'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)
'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)
'Adding a sample value to "A4" cell
worksheet.Cells("A4").PutValue(200)
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'Adding a sample value to "B4" cell
worksheet.Cells("B4").PutValue(40)
'Adding a sample value to "C1" cell as category data
worksheet.Cells("C1").PutValue("Q1")
'Adding a sample value to "C2" cell as category data
worksheet.Cells("C2").PutValue("Q2")
'Adding a sample value to "C3" cell as category data
worksheet.Cells("C3").PutValue("Y1")
'Adding a sample value to "C4" cell as category data
worksheet.Cells("C4").PutValue("Y2")
'Hinzufügen eines Diagramms zum Arbeitsblatt
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Zugriff auf die Instanz des neu hinzugefügten Diagramms
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.NSeries.Add("A1:B4", True)
'Festlegen der Datenquelle für die Kategoriedaten von NSeries
Chart.NSeries.CategoryData = "C1:C4"
'Einstellen der Anzeigeeinheit der Wertachse (Y-Achse).
chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds
Dim displayUnitLabel As DisplayUnitLabel = chart.ValueAxis.DisplayUnitLabel
'Festlegen der Beschriftung der benutzerdefinierten Anzeigeeinheit
displayUnitLabel.Text = "100"
'Speichern der Excel-Datei
workbook.Save("book1.xls")
```

### Siehe auch

* class [ChartTextFrame](../charttextframe)
* namensraum [Aspose.Cells.Charts](../../aspose.cells.charts)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
