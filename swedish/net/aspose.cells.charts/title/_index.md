---
title: Title
second_title: Aspose.Cells för .NET API-referens
description: Kapslar in objektet som representerar titeln på diagrammet eller axeln.
type: docs
weight: 970
url: /sv/net/aspose.cells.charts/title/
---
## Title class

Kapslar in objektet som representerar titeln på diagrammet eller axeln.

```csharp
public class Title : ChartTextFrame
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
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype) { get; set; } | Hämtar och ställer in textens riktning. |
| virtual [Font](../../aspose.cells.charts/chartframe/font) { get; } | Får en[`Font`](../chartframe/font) objekt för det angivna ChartFrame-objektet. |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | Hämtar eller ställer in höjden på ramen i enheter på 1/4000 av sjökortsytan. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Indikerar om diagramramen har automatisk storlek. |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext) { get; set; } | Indikerar att texten genereras automatiskt. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Indikerar om standardpositionen (DefaultX, DefaultY, DefaultWidth och DefaultHeight) är inställda. |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | Indikerar om denna dataetikett har tagits bort. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Indikerar om storleken på tomtområdets storlek inkluderar bockmarkeringarna och axeletiketterna. False anger att storleken ska avgöra storleken på tomtområdet, bockmarkeringarna och axeletiketterna. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Hämtar eller ställer in om en form ska anpassas automatiskt för att helt innehålla texten som beskrivs i den. Automatisk anpassning är när text i en form skalas för att innehålla all text inuti. |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | Hämtar eller ställer in ett värde som anger om texten är radbruten. |
| [IsVisible](../../aspose.cells.charts/title/isvisible) { get; set; } | Representerar om titeln är synlig. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Hämtar och ställer in en referens till kalkylbladet. |
| [OverLay](../../aspose.cells.charts/title/overlay) { get; set; } | Representerar överlagringscentrerad titel på diagrammet utan att ändra storlek på diagrammet. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Representerar textläsordning. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Representerar textrotationsvinkel. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Sant om ramen har en skugga. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Får[`ShapeProperties`](../chartframe/shapeproperties) objekt. |
| override [Text](../../aspose.cells.charts/title/text) { get; set; } | Hämtar eller ställer in texten för displayenhetens etikett. |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment) { get; set; } | Hämtar och ställer in textens horisontella justering. |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment) { get; set; } | Hämtar eller ställer in textens vertikala justering av text. |
| virtual [Width](../../aspose.cells.charts/chartframe/width) { get; set; } | Hämtar eller ställer in ramens bredd i enheter på 1/4000 av sjökortsytan. |
| override [X](../../aspose.cells.charts/title/x) { get; set; } | Hämtar eller ställer in x-koordinaten för det övre vänstra hörnet i enheter på 1/4000 av sjökortsytan. |
| override [Y](../../aspose.cells.charts/title/y) { get; set; } | Hämtar eller ställer in y-koordinaten för det övre vänstra hörnet i enheter på 1/4000 av sjökortsytan. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Characters](../../aspose.cells.charts/title/characters#characters_1)() | Får rik textformatering av denna titel. |
| [Characters](../../aspose.cells.charts/charttextframe/characters)(int, int) | Returnerar ett teckenobjekt som representerar ett teckenintervall i texten. |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Ställ in positionen för ramen till automatisk |

### Exempel

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

//Ställa in titeln på ett diagram
chart.Title.Text = "Title";
//Ställer in teckensnittsfärgen för diagramtiteln till blå
chart.Title.Font.Color = Color.Blue;
//Ställa in titeln på kategoriaxeln i diagrammet
chart.CategoryAxis.Title.Text = "Category";
//Ställa in titeln på värdeaxeln i diagrammet
chart.ValueAxis.Title.Text = "Value";

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

'Ställa in titeln på ett diagram
chart.Title.Text = "Title"
'Ställer in teckensnittsfärgen för diagramtiteln till blå
chart.Title.Font.Color = Color.Blue
'Ställa in titeln på kategoriaxeln i diagrammet
chart.CategoryAxis.Title.Text = "Category"
'Ställa in titeln på värdeaxeln för diagrammet
chart.ValueAxis.Title.Text = "Value"

```

### Se även

* class [ChartTextFrame](../charttextframe)
* namnutrymme [Aspose.Cells.Charts](../../aspose.cells.charts)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
