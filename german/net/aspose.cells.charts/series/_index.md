---
title: Series
second_title: Aspose.Cells für .NET-API-Referenz
description: Kapselt das Objekt das eine einzelne Datenreihe in einem Diagramm darstellt.
type: docs
weight: 820
url: /de/net/aspose.cells.charts/series/
---
## Series class

Kapselt das Objekt, das eine einzelne Datenreihe in einem Diagramm darstellt.

```csharp
public class Series
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Area](../../aspose.cells.charts/series/area) { get; } | Repräsentiert den Hintergrundbereich des Serienobjekts. |
| [Bar3DShapeType](../../aspose.cells.charts/series/bar3dshapetype) { get; set; } | Ruft den 3D-Formtyp ab oder legt ihn fest, der mit dem 3D-Balken- oder Säulendiagramm verwendet wird. |
| [Border](../../aspose.cells.charts/series/border) { get; } | Repräsentiert den Rand des Serienobjekts. |
| [BubbleScale](../../aspose.cells.charts/series/bubblescale) { get; set; } | Ruft den Skalierungsfaktor für Blasen in der angegebenen Diagrammgruppe ab oder legt ihn fest. Dies kann ein ganzzahliger Wert von 0 (null) bis 300 sein, entspricht einem Prozentsatz der Standardgröße. Gilt nur für Blasendiagramme. |
| [BubbleSizes](../../aspose.cells.charts/series/bubblesizes) { get; set; } | Ruft die Blasengrößenwerte der Diagrammreihe ab oder legt sie fest. |
| [CountOfDataValues](../../aspose.cells.charts/series/countofdatavalues) { get; } | Ruft die Anzahl der Datenwerte ab. |
| [DataLabels](../../aspose.cells.charts/series/datalabels) { get; } | Repräsentiert das DataLabels-Objekt für die angegebene ASeries. |
| [DisplayName](../../aspose.cells.charts/series/displayname) { get; } | Ruft den Namen der Reihe ab, der im Diagramm angezeigt wird. |
| [DoughnutHoleSize](../../aspose.cells.charts/series/doughnutholesize) { get; set; } | Gibt die Größe des Lochs in einer Ringdiagrammgruppe zurück oder legt sie fest. Die Lochgröße wird als Prozentsatz der Diagrammgröße ausgedrückt, zwischen 10 und 90 Prozent. |
| [DownBars](../../aspose.cells.charts/series/downbars) { get; } | Gibt a zurück[`DropBars`](../dropbars) Objekt, das die Abwärtsbalken in einem Liniendiagramm darstellt. Gilt nur für Liniendiagramme. |
| [DropLines](../../aspose.cells.charts/series/droplines) { get; } | Gibt a zurück[`Line`](../../aspose.cells.drawing/line) Objekt, das die Falllinien für eine Reihe im Linien- oder Flächendiagramm darstellt. Gilt nur für Linien- oder Flächendiagramme. |
| [Explosion](../../aspose.cells.charts/series/explosion) { get; set; } | Der Abstand eines offenen Tortenstücks von der Mitte des Tortendiagramms wird als Prozentsatz des Tortendurchmessers ausgedrückt. |
| [FirstSliceAngle](../../aspose.cells.charts/series/firstsliceangle) { get; set; } | Liest oder setzt den Winkel des ersten Torten- oder Doughnut-Diagramms in Grad (im Uhrzeigersinn von der Vertikalen). Gilt nur für Kreis-, 3D-Kreis- und Ringdiagramme, 0 bis 360. |
| [GapWidth](../../aspose.cells.charts/series/gapwidth) { get; set; } | Gibt den Abstand zwischen Balken- oder Spaltenclustern als Prozentsatz der Balken- oder Spaltenbreite zurück oder legt ihn fest. Der Wert dieser Eigenschaft muss zwischen 0 und 500 liegen. |
| [Has3DEffect](../../aspose.cells.charts/series/has3deffect) { get; set; } | True, wenn die Reihe dreidimensional aussieht. Gilt nur für Blasendiagramme. |
| [HasDropLines](../../aspose.cells.charts/series/hasdroplines) { get; set; } | Wahr, wenn das Diagramm Falllinien hat. Gilt nur für Liniendiagramme oder Flächendiagramme. |
| [HasHiLoLines](../../aspose.cells.charts/series/hashilolines) { get; set; } | Wahr, wenn das Liniendiagramm Hoch-Tief-Linien hat. Gilt nur für Liniendiagramme. |
| [HasLeaderLines](../../aspose.cells.charts/series/hasleaderlines) { get; set; } | Wahr, wenn die Serie Führungslinien hat. |
| [HasRadarAxisLabels](../../aspose.cells.charts/series/hasradaraxislabels) { get; set; } | Wahr, wenn ein Netzdiagramm Kategorienachsenbeschriftungen hat. Gilt nur für Radarkarten. |
| [HasSeriesLines](../../aspose.cells.charts/series/hasserieslines) { get; set; } | Wahr, wenn ein gestapeltes Säulen- oder Balkendiagramm Reihenlinien aufweist, oder , wenn ein Tortendiagramm oder ein Balkendiagramm Verbindungslinien zwischen den beiden Abschnitten aufweist. Gilt nur für gestapelte Säulendiagramme, Balkendiagramme, Tortendiagramme oder Balkendiagramme. |
| [HasUpDownBars](../../aspose.cells.charts/series/hasupdownbars) { get; set; } | Wahr, wenn ein Liniendiagramm Aufwärts- und Abwärtsbalken hat. Gilt nur für Liniendiagramme. |
| [HiLoLines](../../aspose.cells.charts/series/hilolines) { get; } | Gibt ein HiLoLines-Objekt zurück, das die High-Low-Linien für eine Reihe in einem Liniendiagramm darstellt. Gilt nur für Liniendiagramme. |
| [IsAutoSplit](../../aspose.cells.charts/series/isautosplit) { get; } | Gibt an, ob der Schwellenwert automatisch ist. |
| [IsColorVaried](../../aspose.cells.charts/series/iscolorvaried) { get; set; } | Stellt dar, ob die Farbe der Punkte variiert wird. Das Diagramm darf nur eine Reihe enthalten. |
| [IsVerticalValues](../../aspose.cells.charts/series/isverticalvalues) { get; } | Gibt an, ob die Datenquelle vertikal ist. |
| [LayoutProperties](../../aspose.cells.charts/series/layoutproperties) { get; } | Repräsentiert die Eigenschaften des Layouts. |
| [LeaderLines](../../aspose.cells.charts/series/leaderlines) { get; } | Repräsentiert Führungslinien auf einem Diagramm. Führungslinien verbinden Datenbeschriftungen mit Datenpunkten. Dieses Objekt ist keine Sammlung; Es gibt kein Objekt, das eine einzelne Führungslinie darstellt. |
| [LegendEntry](../../aspose.cells.charts/series/legendentry) { get; } | Ruft den Legendeneintrag gemäß dieser Reihe ab. |
| [Marker](../../aspose.cells.charts/series/marker) { get; } | Ruft die ab[`Marker`](./marker) . |
| [Name](../../aspose.cells.charts/series/name) { get; set; } | Holt oder setzt den Namen der Datenreihe. |
| [Overlap](../../aspose.cells.charts/series/overlap) { get; set; } | Gibt an, wie Balken und Säulen positioniert werden. Kann ein Wert zwischen – 100 und 100 sein. Gilt nur für 2-D-Balken- und 2-D-Säulendiagramme. |
| [PlotOnSecondAxis](../../aspose.cells.charts/series/plotonsecondaxis) { get; set; } | Gibt an, ob diese Reihe auf der zweiten Werteachse aufgetragen wird. |
| [Points](../../aspose.cells.charts/series/points) { get; } | Ruft die Sammlung von Punkten in einer Reihe in einem Diagramm ab. |
| [SecondPlotSize](../../aspose.cells.charts/series/secondplotsize) { get; set; } | Gibt die Größe des sekundären Abschnitts entweder eines Tortendiagramms oder eines Balkendiagramms zurück oder legt sie fest, als Prozentsatz der Größe des primären Tortendiagramms. Kann ein Wert zwischen 5 und 200 sein. |
| [SeriesLines](../../aspose.cells.charts/series/serieslines) { get; } | Gibt ein SeriesLines-Objekt zurück, das die Reihenlinien für ein gestapeltes Balkendiagramm oder ein gestapeltes Säulendiagramm darstellt. Gilt nur für gestapelte Balken- und gestapelte Säulendiagramme. |
| [Shadow](../../aspose.cells.charts/series/shadow) { get; set; } | True, wenn die Serie einen Schatten hat. |
| [ShapeProperties](../../aspose.cells.charts/series/shapeproperties) { get; } | Ruft die ab Objekt, das die visuellen Formeigenschaften der Serie enthält. |
| [ShowNegativeBubbles](../../aspose.cells.charts/series/shownegativebubbles) { get; set; } | Wahr, wenn negative Blasen für die Diagrammgruppe angezeigt werden. Gilt nur für Blasendiagramme. |
| [SizeRepresents](../../aspose.cells.charts/series/sizerepresents) { get; set; } | Ruft ab oder legt fest, was die Blasengröße in einem Blasendiagramm darstellt. |
| [Smooth](../../aspose.cells.charts/series/smooth) { get; set; } | Repräsentiert die Kurvenglättung. Wahr, wenn die Kurvenglättung für das Linien- oder Streudiagramm aktiviert ist. Gilt nur für Linien- und Streudiagramme, die durch Linien verbunden sind. |
| [SplitType](../../aspose.cells.charts/series/splittype) { get; set; } | Gibt einen Wert zurück oder legt einen Wert fest, mit dem bestimmt wird, welche Datenpunkte sich im zweiten Kreis oder Balken auf einem Torten- oder Balkendiagramm von befinden. |
| [SplitValue](../../aspose.cells.charts/series/splitvalue) { get; set; } | Gibt einen Wert zurück oder legt einen Wert fest, der verwendet werden soll, um zu bestimmen, welche Datenpunkte sich im zweiten Kreis oder Balken auf einem Torten- oder Balkendiagramm befinden. |
| [TrendLines](../../aspose.cells.charts/series/trendlines) { get; } | Gibt ein Objekt zurück, das eine Sammlung aller Trendlinien für die Reihe darstellt. |
| [Type](../../aspose.cells.charts/series/type) { get; set; } | Ruft den Typ einer Datenreihe ab oder legt ihn fest. |
| [UpBars](../../aspose.cells.charts/series/upbars) { get; } | Gibt ein DropBars-Objekt zurück, das die Aufwärtsbalken in einem Liniendiagramm darstellt. Gilt nur für Liniendiagramme. |
| [Values](../../aspose.cells.charts/series/values) { get; set; } | Repräsentiert die Daten der Diagrammreihe. |
| [ValuesFormatCode](../../aspose.cells.charts/series/valuesformatcode) { get; set; } | Repräsentiert den Formatcode der NumberList von Values. |
| [XErrorBar](../../aspose.cells.charts/series/xerrorbar) { get; } | Stellt den X-Richtungsfehlerbalken der Serie dar. |
| [XValues](../../aspose.cells.charts/series/xvalues) { get; set; } | Stellt die x-Werte der Diagrammreihe dar. |
| [YErrorBar](../../aspose.cells.charts/series/yerrorbar) { get; } | Repräsentiert den Y-Richtungsfehlerbalken der Serie. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Move](../../aspose.cells.charts/series/move)(int) | Verschiebt die Reihe nach oben oder unten. |

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
int seriesIndex = chart.NSeries.Add("A1:B4", true);
//Festlegen der Datenquelle für die Kategoriedaten von NSeries
chart.NSeries.CategoryData = "C1:C4";
Series series = chart.NSeries[seriesIndex];
//Festlegen der Werte der Reihe.
series.Values = "=B1:B4";
//Ändern des Diagrammtyps der Serie.
series.Type = ChartType.Line;
//Markereigenschaften setzen.
series.Marker.MarkerStyle = ChartMarkerType.Circle;
series.Marker.ForegroundColorSetType = FormattingType.Automatic;
series.Marker.ForegroundColor = System.Drawing.Color.Black;
series.Marker.BackgroundColorSetType = FormattingType.Automatic;

// Mach dein Geschäft

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
Dim seriesIndex As Int32 = chart.NSeries.Add("A1:B4", True)
'Festlegen der Datenquelle für die Kategoriedaten von NSeries
chart.NSeries.CategoryData = "C1:C4"
Dim series As Series = chart.NSeries(seriesIndex)
'Einstellen der Werte der Reihe.
series.Values = "=B1:B4"
'Ändern des Diagrammtyps der Reihe.
series.Type = ChartType.Line
'Markierungseigenschaften festlegen.
series.Marker.MarkerStyle = ChartMarkerType.Circle
series.Marker.ForegroundColorSetType = FormattingType.Automatic
series.Marker.ForegroundColor = System.Drawing.Color.Black
series.Marker.BackgroundColorSetType = FormattingType.Automatic
'Speichern der Excel-Datei
workbook.Save("book1.xls")
```

### Siehe auch

* namensraum [Aspose.Cells.Charts](../../aspose.cells.charts)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
