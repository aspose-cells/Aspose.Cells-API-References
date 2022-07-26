---
title: FillFormat
second_title: Aspose.Cells för .NET API-referens
description: Kapslar in objektet som representerar fyllningsformatering för en form.
type: docs
weight: 1970
url: /sv/net/aspose.cells.drawing/fillformat/
---
## FillFormat class

Kapslar in objektet som representerar fyllningsformatering för en form.

```csharp
public class FillFormat
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [FillType](../../aspose.cells.drawing/fillformat/filltype) { get; set; } | Hämtar och ställer in fyllningstyp |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1) { get; } | Returnerar gradientfärg 1 för den angivna fyllningen. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2) { get; } | Returnerar gradientfärg 2 för den angivna fyllningen. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype) { get; } | Returnerar gradientfärgtypen för den angivna fyllningen. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree) { get; } | Returnerar gradientgraden för den angivna fyllningen. Gäller endast Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill) { get; } | Blir[`GradientFill`](./gradientfill) objekt. |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle) { get; } | Returnerar gradientstilen för den angivna fyllningen. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant) { get; } | Returnerar gradientvarianten för den angivna fyllningen. Gäller endast Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata) { get; set; } | Hämtar och ställer in bildbildsdata. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern) { get; set; } | Representerar ett områdes visningsmönster. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill) { get; } | Blir[`PatternFill`](./patternfill) objekt. |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype) { get; set; } | Hämtar och ställer in bildformatstypen. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor) { get; } | Returnerar den förinställda övertoningsfärgen för den angivna fyllningen. |
| [Scale](../../aspose.cells.drawing/fillformat/scale) { get; set; } | Hämtar och ställer in bildformatsskalan. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill) { get; } | Blir[`SolidFill`](./solidfill) objekt. |
| [Texture](../../aspose.cells.drawing/fillformat/texture) { get; set; } | Representerar texturtypen för den angivna fyllningen. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill) { get; } | Blir[`TextureFill`](./texturefill) objekt. |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency) { get; set; } | Returnerar eller ställer in graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (clear). |

## Metoder

| namn | Beskrivning |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fillformat/equals)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/fillformat/gethashcode)() | Hämtar hashkoden. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient)(Color, double, GradientStyleType, int) | Ställer in den angivna fyllningen till en enfärgsgradient. Gäller endast Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient)(GradientPresetType, GradientStyleType, int) | Ställer in den angivna fyllningen till en förinställd färggradient. Gäller endast Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Ställer in den angivna fyllningen till en tvåfärgsgradient. Gäller endast Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Ställer in den angivna fyllningen till en tvåfärgsgradient. Gäller endast Excel 2007. |

### Exempel

```csharp

[C#]

//Instantiering av ett arbetsboksobjekt
Workbook workbook = new Workbook();
//Lägga till ett nytt kalkylblad till Excel-objektet
int sheetIndex = workbook.Worksheets.Add();
//Hämta referensen till det nyligen tillagda kalkylbladet genom att skicka dess arkindex
Worksheet worksheet = workbook.Worksheets[sheetIndex];
//Lägga till ett exempelvärde i cellen "A1".
worksheet.Cells["A1"].PutValue(50);
//Lägga till ett exempelvärde till "A2"-cellen
worksheet.Cells["A2"].PutValue(100);
//Lägga till ett exempelvärde till "A3"-cellen
worksheet.Cells["A3"].PutValue(150);
//Lägga till ett exempelvärde till "A4"-cellen
worksheet.Cells["A4"].PutValue(200);
//Lägga till ett exempelvärde till "B1"-cellen
worksheet.Cells["B1"].PutValue(60);
//Lägga till ett exempelvärde till "B2"-cellen
worksheet.Cells["B2"].PutValue(32);
//Lägga till ett exempelvärde till "B3"-cellen
worksheet.Cells["B3"].PutValue(50);
//Lägga till ett exempelvärde till "B4"-cellen
worksheet.Cells["B4"].PutValue(40);
//Lägga till ett exempelvärde till "C1"-cellen som kategoridata
worksheet.Cells["C1"].PutValue("Q1");
//Lägga till ett exempelvärde till "C2"-cellen som kategoridata
worksheet.Cells["C2"].PutValue("Q2");
//Lägga till ett exempelvärde till "C3"-cellen som kategoridata
worksheet.Cells["C3"].PutValue("Y1");
//Lägga till ett exempelvärde till "C4"-cellen som kategoridata
worksheet.Cells["C4"].PutValue("Y2");
//Lägga till ett diagram i arbetsbladet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
//Åtkomst till instansen av det nyligen tillagda diagrammet
Chart chart = worksheet.Charts[chartIndex];
//Lägga till NSeries (diagramdatakälla) till diagrammet som sträcker sig från "A1"-cell till "B4"
int seriesIndex = chart.NSeries.Add("A1:B4", true);
//Ställa in datakällan för kategoridata för NSeries
chart.NSeries.CategoryData = "C1:C4";
//Fyllning av området för den 2:a NS-serien med en gradient
chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(Color.Lime, 1, GradientStyleType.Horizontal, 1);

[Visual Basic]

Instantiera ett arbetsboksobjekt
Dim workbook As Workbook = New Workbook()
'Lägga till ett nytt kalkylblad till Excel-objektet
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'Få referensen till det nyligen tillagda kalkylbladet genom att skicka dess arkindex
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
'Lägga till ett diagram i arbetsbladet
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Åtkomst till instansen av det nyligen tillagda diagrammet
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
Dim seriesIndex As Int32 = chart.NSeries.Add("A1:B4", True)
'Ställa in datakällan för kategoridata för NSeries
chart.NSeries.CategoryData = "C1:C4"
'Fyller området för den 2:a NS-serien med en gradient
chart.NSeries(seriesIndex).Area.FillFormat.SetOneColorGradient(Color.Lime, 1, GradientStyleType.Horizontal, 1)
```

### Se även

* namnutrymme [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
