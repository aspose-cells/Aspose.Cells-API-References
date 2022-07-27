---
title: ChartArea
second_title: Aspose.Cells für .NET-API-Referenz
description: Kapselt das Objekt das den Diagrammbereich im Arbeitsblatt darstellt.
type: docs
weight: 440
url: /de/net/aspose.cells.charts/chartarea/
---
## ChartArea class

Kapselt das Objekt, das den Diagrammbereich im Arbeitsblatt darstellt.

```csharp
public class ChartArea : ChartFrame
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
| override [Font](../../aspose.cells.charts/chartarea/font) { get; } | erhält a[`Font`](./font) Objekt des angegebenen Chartarea-Objekts. |
| override [Height](../../aspose.cells.charts/chartarea/height) { get; set; } | Holt oder setzt den vertikalen Abstand von der unteren rechten Eckzeile. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Gibt an, ob die Größe des Diagrammrahmens automatisch angepasst wird. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Gibt an, ob die Standardposition (DefaultX, DefaultY, DefaultWidth und DefaultHeight) eingestellt ist. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Gibt an, ob die Größe des Plotbereichs die Teilstriche und die Achsenbeschriftungen umfasst. False gibt an, dass die Größe die Größe des Plotbereichs, der Teilstriche und der Achsenbeschriftungen bestimmen soll. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | True, wenn der Rahmen einen Schatten hat. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Ruft die ab[`ShapeProperties`](../chartframe/shapeproperties) Objekt. |
| override [Width](../../aspose.cells.charts/chartarea/width) { get; set; } | Ruft den horizontalen Versatz von der Spalte in der unteren rechten Ecke ab oder legt ihn fest. |
| override [X](../../aspose.cells.charts/chartarea/x) { get; set; } | Holt oder bekommt den horizontalen Versatz von seiner oberen linken Eckspalte. |
| override [Y](../../aspose.cells.charts/chartarea/y) { get; set; } | Holt oder bekommt den vertikalen Offset von seiner oberen linken Eckreihe. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Position des Rahmens auf automatisch setzen |

### Beispiele

```csharp

[C#]

//Instanziieren eines Workbook-Objekts
Workbook workbook = new Workbook();

// Abrufen der Referenz des ersten Arbeitsblatts
Worksheet worksheet = workbook.Worksheets[0];

//Hinzufügen eines Beispielwerts zur Zelle "A1".
worksheet.Cells["A1"].PutValue(50);

//Hinzufügen eines Beispielwerts zur Zelle "A2".
worksheet.Cells["A2"].PutValue(100);

//Hinzufügen eines Beispielwerts zur Zelle "A3".
worksheet.Cells["A3"].PutValue(150);

//Hinzufügen eines Beispielwerts zur Zelle "B1".
worksheet.Cells["B1"].PutValue(60);

//Hinzufügen eines Beispielwerts zur Zelle "B2".
worksheet.Cells["B2"].PutValue(32);

//Hinzufügen eines Beispielwerts zur Zelle "B3".
worksheet.Cells["B3"].PutValue(50);

//Hinzufügen eines Diagramms zum Arbeitsblatt
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);

//Auf die Instanz des neu hinzugefügten Diagramms zugreifen
Chart chart = worksheet.Charts[chartIndex];

//Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm im Bereich von Zelle "A1" bis "B3"
chart.NSeries.Add("A1:B3", true);

//Diagrammbereich abrufen
ChartArea chartArea = chart.ChartArea;

//Festlegen der Vordergrundfarbe des Diagrammbereichs
chartArea.Area.ForegroundColor = Color.Yellow;

//Schatten des Diagrammbereichs einstellen
chartArea.Shadow = true;

//Speichern der Excel-Datei
workbook.Save("book1.xls");

[VB.NET]

'Instanziieren eines Workbook-Objekts
Dim workbook As Workbook = New Workbook()

'Abrufen der Referenz des ersten Arbeitsblatts
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)

'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)

'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)

'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)

'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)

'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)

'Hinzufügen eines Diagramms zum Arbeitsblatt
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)

'Zugriff auf die Instanz des neu hinzugefügten Diagramms
Dim chart As Chart = worksheet.Charts(chartIndex)

'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", True)

'Kartenbereich abrufen
Dim chartArea As ChartArea = chart.ChartArea

'Festlegen der Vordergrundfarbe des Diagrammbereichs
chartArea.Area.ForegroundColor = Color.Yellow

'Schatten des Diagrammbereichs einstellen
chartArea.Shadow = True

'Speichern der Excel-Datei
workbook.Save("book1.xls")
```

### Siehe auch

* class [ChartFrame](../chartframe)
* namensraum [Aspose.Cells.Charts](../../aspose.cells.charts)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
