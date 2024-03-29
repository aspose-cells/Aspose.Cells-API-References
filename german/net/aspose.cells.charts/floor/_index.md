---
title: Floor
second_title: Aspose.Cells für .NET-API-Referenz
description: Kapselt das Objekt das den Boden eines 3D-Diagramms darstellt.
type: docs
weight: 660
url: /de/net/aspose.cells.charts/floor/
---
## Floor class

Kapselt das Objekt, das den Boden eines 3D-Diagramms darstellt.

```csharp
public class Floor : Area
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor) { get; set; } | Holt oder setzt den HintergrundColor des[`Area`](../../aspose.cells.drawing/area) . |
| [Border](../../aspose.cells.charts/floor/border) { get; set; } | Holt oder setzt die Grenze[`Line`](../../aspose.cells.drawing/line) . |
| [FillFormat](../../aspose.cells.drawing/area/fillformat) { get; } | steht für a Objekt, das Füllformatierungseigenschaften für das angegebene Diagramm oder die angegebene Form enthält. |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor) { get; set; } | Holt oder setzt den VordergrundColor . |
| [Formatting](../../aspose.cells.drawing/area/formatting) { get; set; } | Stellt die Formatierung des Bereichs dar. |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative) { get; set; } | Wenn die Eigenschaft wahr ist und der Wert des Diagrammpunkts eine negative Zahl ist, werden Vorder- und Hintergrundfarbe ausgetauscht. |
| [Transparency](../../aspose.cells.drawing/area/transparency) { get; set; } | Gibt den Transparenzgrad des Bereichs als Wert von 0,0 (deckend) bis 1,0 (klar) zurück oder legt ihn fest. |

### Beispiele

```csharp

[C#]

//Instanziieren Sie die Lizenzklasse
Aspose.Cells.License license = new Aspose.Cells.License();

//Übergeben Sie nur den Namen der in die Assembly eingebetteten Lizenzdatei
license.SetLicense("Aspose.Cells.lic");

//Das Arbeitsmappenobjekt instanziieren
Workbook workbook = new Workbook();

// Zellensammlung abrufen
Cells cells = workbook.Worksheets[0].Cells;

//Werte in Zellen einfügen
cells["A1"].PutValue(1);

cells["A2"].PutValue(2);

cells["A3"].PutValue(3);

// Diagrammsammlung abrufen
ChartCollection charts = workbook.Worksheets[0].Charts;

// neues Diagramm hinzufügen 
int index = charts.Add(ChartType.Column3DStacked, 5, 0, 15, 5);

// Holen Sie sich das neu hinzugefügte Diagramm
Chart chart = charts[index];

//Charts nseries setzen
chart.NSeries.Add("A1:A3", true);

//Datenbeschriftungen anzeigen
chart.NSeries[0].DataLabels.ShowValue = true;

// Holen Sie sich den Boden des Diagramms
Floor floor = chart.Floor;

// Setzen Sie die Grenze des Bodens auf Rot
floor.Border.Color = System.Drawing.Color.Red;

// Füllformat festlegen
floor.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.DiagonalDown, 2); 

//Speicher die Datei
workbook.Save(@"dest.xls");

[VB.NET]

'Instanziieren Sie die License-Klasse
Dim license As New Aspose.Cells.License()

'Übergeben Sie nur den Namen der in die Assembly eingebetteten Lizenzdatei
license.SetLicense("Aspose.Cells.lic")

'Instanziieren Sie das Arbeitsmappenobjekt
Dim workbook As Workbook = New Workbook()

'Holen Sie sich die Zellensammlung
Dim cells As Cells = workbook.Worksheets(0).Cells

'Trage Werte in Zellen ein
cells("A1").PutValue(1)

cells("A2").PutValue(2)

cells("A3").PutValue(3)

'Holen Sie sich eine Diagrammsammlung
Dim charts As ChartCollection = workbook.Worksheets(0).Charts

'füge ein neues Diagramm hinzu 
Dim index As Integer = charts.Add(ChartType.Column3DStacked, 5, 0, 15, 5)

'Holen Sie sich das neu hinzugefügte Diagramm
Dim chart As Chart = charts(index)

'set charts nseries
chart.NSeries.Add("A1:A3", True)

'Datenbeschriftungen anzeigen
chart.NSeries(0).DataLabels.ShowValue = True

'Get chart's floor
Dim floor As Floor = chart.Floor

'set floor's border as red
floor.Border.Color = System.Drawing.Color.Red

'Füllformat festlegen
floor.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.DiagonalDown, 2)

'Speicher die Datei
workbook.Save("dest.xls")

```

### Siehe auch

* class [Area](../../aspose.cells.drawing/area)
* namensraum [Aspose.Cells.Charts](../../aspose.cells.charts)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
