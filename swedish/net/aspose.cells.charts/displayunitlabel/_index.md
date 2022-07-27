---
title: DisplayUnitLabel
second_title: Aspose.Cells för .NET API-referens
description: Representerar displayenhetens etikett.
type: docs
weight: 600
url: /sv/net/aspose.cells.charts/displayunitlabel/
---
## DisplayUnitLabel class

Representerar displayenhetens etikett.

```csharp
public class DisplayUnitLabel : ChartTextFrame
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | Får[`område`](../chartframe/area) . |
| override [AutoScaleFont](../../aspose.cells.charts/displayunitlabel/autoscalefont) { get; set; } | Sant om texten i objektet ändrar teckenstorlek när objektstorleken ändras. Standardvärdet är True. |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | Hämtar och ställer in visningsläget för bakgrunden |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | Får[`gräns`](../../aspose.cells.drawing/line) . |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Representerar höjden på standardpositionen |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Representerar bredden på standardposition |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Representerar x av standardposition |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Representerar y för standardposition |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype) { get; set; } | Hämtar och ställer in textens riktning. |
| override [Font](../../aspose.cells.charts/displayunitlabel/font) { get; } | Får en[`Font`](./font) objekt för det angivna ChartFrame-objektet. |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | Hämtar eller ställer in höjden på ramen i enheter på 1/4000 av sjökortsytan. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Indikerar om diagramramen har automatisk storlek. |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext) { get; set; } | Indikerar att texten genereras automatiskt. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Indikerar om standardpositionen (DefaultX, DefaultY, DefaultWidth och DefaultHeight) är inställda. |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | Indikerar om denna dataetikett har tagits bort. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Indikerar om storleken på tomtområdets storlek inkluderar bockmarkeringarna och axeletiketterna. False anger att storleken ska avgöra storleken på tomtområdet, bockmarkeringarna och axeletiketterna. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Hämtar eller ställer in om en form ska anpassas automatiskt för att helt innehålla texten som beskrivs i den. Automatisk anpassning är när text i en form skalas för att innehålla all text inuti. |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | Hämtar eller ställer in ett värde som anger om texten är radbruten. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Hämtar och ställer in en referens till kalkylbladet. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Representerar textläsordning. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Representerar textrotationsvinkel. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Sant om ramen har en skugga. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Får[`ShapeProperties`](../chartframe/shapeproperties) objekt. |
| override [Text](../../aspose.cells.charts/displayunitlabel/text) { get; set; } | Hämtar eller ställer in texten för displayenhetens etikett. |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment) { get; set; } | Hämtar och ställer in textens horisontella justering. |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment) { get; set; } | Hämtar eller ställer in textens vertikala justering av text. |
| virtual [Width](../../aspose.cells.charts/chartframe/width) { get; set; } | Hämtar eller ställer in ramens bredd i enheter på 1/4000 av sjökortsytan. |
| virtual [X](../../aspose.cells.charts/chartframe/x) { get; set; } | Hämtar eller ställer in x-koordinaten för det övre vänstra hörnet i enheter på 1/4000 av sjökortsytan. |
| virtual [Y](../../aspose.cells.charts/chartframe/y) { get; set; } | Hämtar eller ställer in y-koordinaten för det övre vänstra hörnet i enheter på 1/4000 av sjökortsytan. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Characters](../../aspose.cells.charts/charttextframe/characters)(int, int) | Returnerar ett teckenobjekt som representerar ett teckenintervall i texten. |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Ställ in positionen för ramen till automatisk |

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
chart.NSeries.Add("A1:B4", true);
//Ställa in datakällan för kategoridata för NSeries
chart.NSeries.CategoryData = "C1:C4";
//Ställa in displayenheten för värde(Y)-axeln.
chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
DisplayUnitLabel displayUnitLabel = chart.ValueAxis.DisplayUnitLabel;
//Ställa in etiketten för anpassad displayenhet
displayUnitLabel.Text = "100";
//Spara Excel-filen
workbook.Save("book1.xls");

[Visual Basic]

'Instantiera ett arbetsboksobjekt
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
chart.NSeries.Add("A1:B4", True)
'Ställa in datakällan för kategoridata för NSeries
Chart.NSeries.CategoryData = "C1:C4"
'Ställa in displayenheten för värde(Y)-axeln.
chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds
Dim displayUnitLabel As DisplayUnitLabel = chart.ValueAxis.DisplayUnitLabel
'Ställa in etiketten för anpassad displayenhet
displayUnitLabel.Text = "100"
'Sparar Excel-filen
workbook.Save("book1.xls")
```

### Se även

* class [ChartTextFrame](../charttextframe)
* namnutrymme [Aspose.Cells.Charts](../../aspose.cells.charts)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
