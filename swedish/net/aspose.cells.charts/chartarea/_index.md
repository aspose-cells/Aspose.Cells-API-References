---
title: ChartArea
second_title: Aspose.Cells för .NET API-referens
description: Kapslar in objektet som representerar diagramområdet i kalkylbladet.
type: docs
weight: 440
url: /sv/net/aspose.cells.charts/chartarea/
---
## ChartArea class

Kapslar in objektet som representerar diagramområdet i kalkylbladet.

```csharp
public class ChartArea : ChartFrame
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | Får[`område`](../chartframe/area) . |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont) { get; set; } | Sant om texten i objektet ändrar teckenstorlek när objektstorleken ändras. Standardvärdet är True. |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | Hämtar och ställer in visningsläget för bakgrunden |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | Får[`gräns`](../../aspose.cells.drawing/line) . |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Representerar höjden på standardpositionen |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Representerar bredden på standardposition |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Representerar x av standardposition |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Representerar y för standardposition |
| override [Font](../../aspose.cells.charts/chartarea/font) { get; } | Får en[`Font`](./font) objekt för det angivna chartarea-objektet. |
| override [Height](../../aspose.cells.charts/chartarea/height) { get; set; } | Hämtar eller ställer in den vertikala offseten från dess nedre högra hörnrad. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Indikerar om diagramramen har automatisk storlek. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Indikerar om standardpositionen (DefaultX, DefaultY, DefaultWidth och DefaultHeight) är inställda. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Indikerar om storleken på tomtområdets storlek inkluderar bockmarkeringarna och axeletiketterna. False anger att storleken ska avgöra storleken på tomtområdet, bockmarkeringarna och axeletiketterna. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Sant om ramen har en skugga. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Får[`ShapeProperties`](../chartframe/shapeproperties) objekt. |
| override [Width](../../aspose.cells.charts/chartarea/width) { get; set; } | Hämtar eller ställer in den horisontella offseten från kolumnen i det nedre högra hörnet. |
| override [X](../../aspose.cells.charts/chartarea/x) { get; set; } | Hämtar eller hämtar den horisontella förskjutningen från kolumnen i det övre vänstra hörnet. |
| override [Y](../../aspose.cells.charts/chartarea/y) { get; set; } | Hämtar eller hämtar den vertikala offseten från dess övre vänstra hörnrad. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Ställ in positionen för ramen till automatisk |

### Exempel

```csharp

[C#]

//Instantiering av ett arbetsboksobjekt
Workbook workbook = new Workbook();

//Hämta referensen till det första kalkylbladet
Worksheet worksheet = workbook.Worksheets[0];

//Lägga till ett exempelvärde i cellen "A1".
worksheet.Cells["A1"].PutValue(50);

//Lägga till ett exempelvärde till "A2"-cellen
worksheet.Cells["A2"].PutValue(100);

//Lägga till ett exempelvärde till "A3"-cellen
worksheet.Cells["A3"].PutValue(150);

//Lägga till ett exempelvärde till "B1"-cellen
worksheet.Cells["B1"].PutValue(60);

//Lägga till ett exempelvärde till "B2"-cellen
worksheet.Cells["B2"].PutValue(32);

//Lägga till ett exempelvärde till "B3"-cellen
worksheet.Cells["B3"].PutValue(50);

//Lägga till ett diagram i arbetsbladet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);

//Åtkomst till instansen av det nyligen tillagda diagrammet
Chart chart = worksheet.Charts[chartIndex];

//Lägga till NSeries (diagramdatakälla) till diagrammet som sträcker sig från "A1"-cell till "B3"
chart.NSeries.Add("A1:B3", true);

//Hämta sjökortsområde
ChartArea chartArea = chart.ChartArea;

//Ställa in förgrundsfärgen för diagramområdet
chartArea.Area.ForegroundColor = Color.Yellow;

//Ställa in diagramområdesskugga
chartArea.Shadow = true;

//Spara Excel-filen
workbook.Save("book1.xls");

[VB.NET]

'Instantiera ett arbetsboksobjekt
Dim workbook As Workbook = New Workbook()

'Få referensen till det första arbetsbladet
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

'Lägga till ett diagram i arbetsbladet
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)

'Åtkomst till instansen av det nyligen tillagda diagrammet
Dim chart As Chart = worksheet.Charts(chartIndex)

'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", True)

'Får sjökortsområde
Dim chartArea As ChartArea = chart.ChartArea

'Ställa in förgrundsfärgen för diagramområdet
chartArea.Area.ForegroundColor = Color.Yellow

'Ställa in diagramområdesskugga
chartArea.Shadow = True

'Sparar Excel-filen
workbook.Save("book1.xls")
```

### Se även

* class [ChartFrame](../chartframe)
* namnutrymme [Aspose.Cells.Charts](../../aspose.cells.charts)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
