---
title: FillFormat
second_title: Aspose.Cells für .NET-API-Referenz
description: Kapselt das Objekt das die Füllformatierung für eine Form darstellt.
type: docs
weight: 1970
url: /de/net/aspose.cells.drawing/fillformat/
---
## FillFormat class

Kapselt das Objekt, das die Füllformatierung für eine Form darstellt.

```csharp
public class FillFormat
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [FillType](../../aspose.cells.drawing/fillformat/filltype) { get; set; } | Ruft Fülltyp ab und legt ihn fest |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1) { get; } | Gibt die Verlaufsfarbe 1 für die angegebene Füllung zurück. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2) { get; } | Gibt die Verlaufsfarbe 2 für die angegebene Füllung zurück. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype) { get; } | Gibt den Verlaufsfarbtyp für die angegebene Füllung zurück. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree) { get; } | Gibt den Gradientengrad für die angegebene Füllung zurück. Gilt nur für Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill) { get; } | erhält[`GradientFill`](./gradientfill) Objekt. |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle) { get; } | Gibt den Verlaufsstil für die angegebene Füllung zurück. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant) { get; } | Gibt die Verlaufsvariante für die angegebene Füllung zurück. Gilt nur für Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata) { get; set; } | Ruft die Bilddaten ab und legt sie fest. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern) { get; set; } | Repräsentiert das Anzeigemuster eines Bereichs. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill) { get; } | erhält[`PatternFill`](./patternfill) Objekt. |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype) { get; set; } | Ruft den Bildformattyp ab und legt ihn fest. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor) { get; } | Gibt die voreingestellte Verlaufsfarbe für die angegebene Füllung zurück. |
| [Scale](../../aspose.cells.drawing/fillformat/scale) { get; set; } | Ruft die Bildformatskalierung ab und legt sie fest. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill) { get; } | erhält[`SolidFill`](./solidfill) Objekt. |
| [Texture](../../aspose.cells.drawing/fillformat/texture) { get; set; } | Repräsentiert den Texturtyp für die angegebene Füllung. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill) { get; } | erhält[`TextureFill`](./texturefill) Objekt. |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency) { get; set; } | Gibt den Transparenzgrad des Bereichs als Wert von 0,0 (deckend) bis 1,0 (klar) zurück oder legt ihn fest. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fillformat/equals)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/fillformat/gethashcode)() | Ruft den Hash-Code ab. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient)(Color, double, GradientStyleType, int) | Legt die angegebene Füllung auf einen einfarbigen Farbverlauf fest. Gilt nur für Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient)(GradientPresetType, GradientStyleType, int) | Legt die angegebene Füllung auf einen voreingestellten Farbverlauf fest. Gilt nur für Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Legt die angegebene Füllung auf einen zweifarbigen Farbverlauf fest. Gilt nur für Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Legt die angegebene Füllung auf einen zweifarbigen Farbverlauf fest. Gilt nur für Excel 2007. |

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
//Füllen Sie den Bereich der 2. NSeries mit einem Farbverlauf
chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(Color.Lime, 1, GradientStyleType.Horizontal, 1);

[Visual Basic]

Instanziieren eines Workbook-Objekts
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
'Füllen Sie den Bereich der 2. NSeries mit einem Farbverlauf
chart.NSeries(seriesIndex).Area.FillFormat.SetOneColorGradient(Color.Lime, 1, GradientStyleType.Horizontal, 1)
```

### Siehe auch

* namensraum [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
