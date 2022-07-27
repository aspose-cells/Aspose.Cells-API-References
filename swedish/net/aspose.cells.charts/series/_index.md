---
title: Series
second_title: Aspose.Cells för .NET API-referens
description: Kapslar in objektet som representerar en enskild dataserie i ett diagram.
type: docs
weight: 820
url: /sv/net/aspose.cells.charts/series/
---
## Series class

Kapslar in objektet som representerar en enskild dataserie i ett diagram.

```csharp
public class Series
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Area](../../aspose.cells.charts/series/area) { get; } | Representerar bakgrundsområdet för serieobjekt. |
| [Bar3DShapeType](../../aspose.cells.charts/series/bar3dshapetype) { get; set; } | Hämtar eller ställer in 3D-formtypen som används med 3D-stapel- eller kolumndiagrammet. |
| [Border](../../aspose.cells.charts/series/border) { get; } | Representerar kantlinjen för serieobjekt. |
| [BubbleScale](../../aspose.cells.charts/series/bubblescale) { get; set; } | Hämtar eller ställer in skalfaktorn för bubblor i den angivna diagramgruppen. Det kan vara ett heltalsvärde från 0 (noll) till 300, motsvarar en procentandel av standardstorleken. Gäller endast bubbeldiagram. |
| [BubbleSizes](../../aspose.cells.charts/series/bubblesizes) { get; set; } | Hämtar eller ställer in bubbelstorlekarna för diagramserien. |
| [CountOfDataValues](../../aspose.cells.charts/series/countofdatavalues) { get; } | Hämtar antalet datavärden. |
| [DataLabels](../../aspose.cells.charts/series/datalabels) { get; } | Representerar DataLabels-objektet för den angivna ASerien. |
| [DisplayName](../../aspose.cells.charts/series/displayname) { get; } | Hämtar seriens namn som visas på diagrammet. |
| [DoughnutHoleSize](../../aspose.cells.charts/series/doughnutholesize) { get; set; } | Returnerar eller ställer in storleken på hålet i en munkdiagramgrupp. Hålstorleken uttrycks som en procentandel av diagramstorleken, mellan 10 och 90 procent. |
| [DownBars](../../aspose.cells.charts/series/downbars) { get; } | Returnerar en[`DropBars`](../dropbars) objekt som representerar nedstaplarna på ett linjediagram. Gäller endast linjediagram. |
| [DropLines](../../aspose.cells.charts/series/droplines) { get; } | Returnerar en[`Line`](../../aspose.cells.drawing/line) objekt som representerar falllinjerna för en serie på linjediagrammet eller ytdiagrammet. Gäller endast linjediagram eller områdesdiagram. |
| [Explosion](../../aspose.cells.charts/series/explosion) { get; set; } | Avståndet för en öppen pajskiva från mitten av cirkeldiagrammet uttrycks i procent av pajdiametern. |
| [FirstSliceAngle](../../aspose.cells.charts/series/firstsliceangle) { get; set; } | Hämtar eller ställer in vinkeln för det första cirkeldiagrammet eller munkdiagrammet, i grader (medsols från lodrät). Gäller endast paj-, 3D-paj- och munkdiagram, 0 till 360. |
| [GapWidth](../../aspose.cells.charts/series/gapwidth) { get; set; } | Returnerar eller ställer in utrymmet mellan stapel- eller kolumnkluster, som en procentandel av stapel- eller kolumnbredden. Värdet på den här egenskapen måste vara mellan 0 och 500. |
| [Has3DEffect](../../aspose.cells.charts/series/has3deffect) { get; set; } | Sant om serien har ett tredimensionellt utseende. Gäller endast bubbeldiagram. |
| [HasDropLines](../../aspose.cells.charts/series/hasdroplines) { get; set; } | Sant om diagrammet har falllinjer. Gäller endast linjediagram eller områdesdiagram. |
| [HasHiLoLines](../../aspose.cells.charts/series/hashilolines) { get; set; } | Sant om linjediagrammet har hög-låg linjer. Gäller endast linjediagram. |
| [HasLeaderLines](../../aspose.cells.charts/series/hasleaderlines) { get; set; } | Sant om serien har ledarlinjer. |
| [HasRadarAxisLabels](../../aspose.cells.charts/series/hasradaraxislabels) { get; set; } | Sant om ett radardiagram har kategoriaxeletiketter. Gäller endast radarsjökort. |
| [HasSeriesLines](../../aspose.cells.charts/series/hasserieslines) { get; set; } | Sant om ett staplat kolumndiagram eller stapeldiagram har serielinjer eller om ett cirkeldiagram eller ett stapeldiagram har kopplingslinjer mellan de två sektionerna. Gäller endast staplade kolumndiagram, stapeldiagram, cirkeldiagram eller stapeldiagram. |
| [HasUpDownBars](../../aspose.cells.charts/series/hasupdownbars) { get; set; } | Sant om ett linjediagram har staplar upp och ner. Gäller endast linjediagram. |
| [HiLoLines](../../aspose.cells.charts/series/hilolines) { get; } | Returnerar ett HiLoLines-objekt som representerar hög-låg-linjerna för en serie på ett linjediagram. Gäller endast linjediagram. |
| [IsAutoSplit](../../aspose.cells.charts/series/isautosplit) { get; } | Indikerar om tröskelvärdet är automatiskt. |
| [IsColorVaried](../../aspose.cells.charts/series/iscolorvaried) { get; set; } | Representerar om färgen på punkter varieras. Diagrammet får endast innehålla en serie. |
| [IsVerticalValues](../../aspose.cells.charts/series/isverticalvalues) { get; } | Indikerar om datakällan är vertikal. |
| [LayoutProperties](../../aspose.cells.charts/series/layoutproperties) { get; } | Representerar egenskaperna för layout. |
| [LeaderLines](../../aspose.cells.charts/series/leaderlines) { get; } | Representerar ledarlinjer på ett diagram. Ledarlinjer kopplar dataetiketter till datapunkter. Detta objekt är inte en samling; det finns inget objekt som representerar en enda ledarlinje. |
| [LegendEntry](../../aspose.cells.charts/series/legendentry) { get; } | Hämtar förklaringsposten enligt denna serie. |
| [Marker](../../aspose.cells.charts/series/marker) { get; } | Får[`markör`](./marker) . |
| [Name](../../aspose.cells.charts/series/name) { get; set; } | Hämtar eller ställer in namnet på dataserien. |
| [Overlap](../../aspose.cells.charts/series/overlap) { get; set; } | Anger hur staplar och kolumner är placerade. Kan vara ett värde mellan – 100 och 100. Gäller endast för 2-D stapel- och 2-D kolumndiagram. |
| [PlotOnSecondAxis](../../aspose.cells.charts/series/plotonsecondaxis) { get; set; } | Indikerar om denna serie är plottad på andra värdeaxeln. |
| [Points](../../aspose.cells.charts/series/points) { get; } | Får samlingen av poäng i en serie i ett diagram. |
| [SecondPlotSize](../../aspose.cells.charts/series/secondplotsize) { get; set; } | Returnerar eller ställer in storleken på den sekundära delen av antingen ett cirkeldiagram eller ett cirkeldiagram, som en procentandel av storleken på den primära cirkeln. Kan vara ett värde från 5 till 200. |
| [SeriesLines](../../aspose.cells.charts/series/serieslines) { get; } | Returnerar ett SeriesLines-objekt som representerar serielinjerna för ett staplat stapeldiagram eller ett staplat kolumndiagram. Gäller endast staplade stapel- och staplade kolumndiagram. |
| [Shadow](../../aspose.cells.charts/series/shadow) { get; set; } | Sant om serien har en skugga. |
| [ShapeProperties](../../aspose.cells.charts/series/shapeproperties) { get; } | Får objekt som har de visuella formegenskaperna för Series. |
| [ShowNegativeBubbles](../../aspose.cells.charts/series/shownegativebubbles) { get; set; } | Sant om negativa bubblor visas för diagramgruppen. Gäller endast för bubbeldiagram. |
| [SizeRepresents](../../aspose.cells.charts/series/sizerepresents) { get; set; } | Hämtar eller ställer in vad bubbelstorleken representerar på ett bubbeldiagram. |
| [Smooth](../../aspose.cells.charts/series/smooth) { get; set; } | Representerar kurvutjämning. Sant om kurvutjämning är aktiverat för linjediagrammet eller punktdiagrammet. Gäller endast linje och spridning kopplade av linjediagram. |
| [SplitType](../../aspose.cells.charts/series/splittype) { get; set; } | Returnerar eller ställer in ett värde som bestämmer vilka datapunkter som finns i den andra cirkeln eller stapeln på en cirkel av cirkel eller stapel av cirkeldiagram. |
| [SplitValue](../../aspose.cells.charts/series/splitvalue) { get; set; } | Returnerar eller ställer in ett värde som ska användas för att bestämma vilka datapunkter som finns i den andra cirkeln eller stapeln on en cirkel av cirkel eller stapel av cirkeldiagram. |
| [TrendLines](../../aspose.cells.charts/series/trendlines) { get; } | Returnerar ett objekt som representerar en samling av alla trendlinjer för serien. |
| [Type](../../aspose.cells.charts/series/type) { get; set; } | Hämtar eller ställer in en dataseries typ. |
| [UpBars](../../aspose.cells.charts/series/upbars) { get; } | Returnerar ett DropBars-objekt som representerar uppstaplarna på ett linjediagram. Gäller endast linjediagram. |
| [Values](../../aspose.cells.charts/series/values) { get; set; } | Representerar data för diagramserien. |
| [ValuesFormatCode](../../aspose.cells.charts/series/valuesformatcode) { get; set; } | Representerar formatkoden för Values NumberList. |
| [XErrorBar](../../aspose.cells.charts/series/xerrorbar) { get; } | Representerar X-riktningsfelfältet i serien. |
| [XValues](../../aspose.cells.charts/series/xvalues) { get; set; } | Representerar x-värdena för diagramserien. |
| [YErrorBar](../../aspose.cells.charts/series/yerrorbar) { get; } | Representerar Y-riktningsfelfältet i serien. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Move](../../aspose.cells.charts/series/move)(int) | Flyttar serien uppåt eller nedåt. |

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
Series series = chart.NSeries[seriesIndex];
//Ställa in värdena för serien.
series.Values = "=B1:B4";
//Ändra diagramtypen för serien.
series.Type = ChartType.Line;
//Ställa in marköregenskaper.
series.Marker.MarkerStyle = ChartMarkerType.Circle;
series.Marker.ForegroundColorSetType = FormattingType.Automatic;
series.Marker.ForegroundColor = System.Drawing.Color.Black;
series.Marker.BackgroundColorSetType = FormattingType.Automatic;

//gör dina affärer

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
Dim seriesIndex As Int32 = chart.NSeries.Add("A1:B4", True)
'Ställa in datakällan för kategoridata för NSeries
chart.NSeries.CategoryData = "C1:C4"
Dim series As Series = chart.NSeries(seriesIndex)
'Ställa in värden för serien.
series.Values = "=B1:B4"
'Ändra diagramtypen för serien.
series.Type = ChartType.Line
'Ställa in marköregenskaper.
series.Marker.MarkerStyle = ChartMarkerType.Circle
series.Marker.ForegroundColorSetType = FormattingType.Automatic
series.Marker.ForegroundColor = System.Drawing.Color.Black
series.Marker.BackgroundColorSetType = FormattingType.Automatic
'Sparar Excel-filen
workbook.Save("book1.xls")
```

### Se även

* namnutrymme [Aspose.Cells.Charts](../../aspose.cells.charts)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
