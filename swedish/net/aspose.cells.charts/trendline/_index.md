---
title: Trendline
second_title: Aspose.Cells för .NET API-referens
description: Representerar en trendlinje i ett diagram.
type: docs
weight: 980
url: /sv/net/aspose.cells.charts/trendline/
---
## Trendline class

Representerar en trendlinje i ett diagram.

```csharp
public class Trendline : Line
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Backward](../../aspose.cells.charts/trendline/backward) { get; set; } | Returnerar eller ställer in antalet perioder (eller enheter på ett punktdiagram) som trendlinjen sträcker sig bakåt. Antalet perioder måste vara större än eller lika med noll. Om diagramtypen är kolumn måste antalet perioder vara mellan 0 och 0,5 |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | Anger längden på pilspetsen för början av en linje. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | Anger bredden på pilspetsen för början av en linje. |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | Anger en pilspets för början av en rad. |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | Anger slutbeteckningar. |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | RepresenterarColor av linjen. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | Anger den sammansatta linjetypen |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | Anger strecklinjetypen |
| [DataLabels](../../aspose.cells.charts/trendline/datalabels) { get; } | Representerar DataLabels-objektet för den angivna serien. |
| [DisplayEquation](../../aspose.cells.charts/trendline/displayequation) { get; set; } | Representerar om ekvationen för trendlinjen visas i diagrammet (i samma dataetikett som R-kvadratvärdet). Om du ställer in den här egenskapen till True aktiveras dataetiketter automatiskt. |
| [DisplayRSquared](../../aspose.cells.charts/trendline/displayrsquared) { get; set; } | Representerar om trendlinjens R-kvadratvärde visas i diagrammet (i samma dataetikett som ekvationen). Om du ställer in den här egenskapen till True aktiveras dataetiketter automatiskt. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | Anger längden på pilspetsen för slutet av en linje. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | Anger bredden på pilspetsen för slutet av en linje. |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | Anger en pilspets för slutet av en rad. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | Hämtar eller ställer in formattyp. |
| [Forward](../../aspose.cells.charts/trendline/forward) { get; set; } | Returnerar eller ställer in antalet perioder (eller enheter på ett punktdiagram) som trendlinjen sträcker sig framåt. Antalet perioder måste vara större än eller lika med noll. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | Representerar gradientfyllning. |
| [Intercept](../../aspose.cells.charts/trendline/intercept) { get; set; } | Returnerar eller ställer in punkten där trendlinjen korsar värdeaxeln. |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | Indikerar om denna linjestil är automatiskt tilldelad. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | Indikerar om färgen på linjen är automatiskt tilldelad. |
| [IsNameAuto](../../aspose.cells.charts/trendline/isnameauto) { get; set; } | Returnerar om Microsoft Excel automatiskt bestämmer namnet på trendlinjen. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | Representerar om linjen är synlig. |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | Anger sammanfogningskapslarna. |
| [LegendEntry](../../aspose.cells.charts/trendline/legendentry) { get; } | Hämtar förklaringsposten enligt denna trendline |
| [Name](../../aspose.cells.charts/trendline/name) { get; set; } | Returnerar namnet på trendlinjen. |
| [Order](../../aspose.cells.charts/trendline/order) { get; set; } | Returnerar eller ställer in trendlinjeordningen (ett heltal större än 1) när trendlinjetypen är polynom. Beställningen måste vara mellan 2 och 6. |
| [Period](../../aspose.cells.charts/trendline/period) { get; set; } | Returnerar eller ställer in perioden för trendlinjen för glidande medelvärde. |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | Representerar stilen på linjen. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | Hämtar och ställer in temafärgen. |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | Returnerar eller ställer in graden av genomskinlighet för linjen som ett värde från 0,0 (ogenomskinlig) till 1,0 (ren). |
| [Type](../../aspose.cells.charts/trendline/type) { get; } | Returnerar trendlinjetypen. |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | Hämtar eller ställer in[`WeightType`](../../aspose.cells.drawing/weighttype) av linjen. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | Hämtar eller ställer in linjens vikt i poängenhet. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | Hämtar eller ställer in linjens vikt i pixelenhet. |

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
//att lägga till en linjär trendlinje
int index = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
Trendline trendline = chart.NSeries[0].TrendLines[index];
//Ställa in det anpassade namnet på trendlinjen.
trendline.Name = "Linear";
//Visar ekvationen på diagrammet
trendline.DisplayEquation = true;
//Visar R-kvadrat-värdet på diagrammet
trendline.DisplayRSquared = true;
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
'lägga till en linjär trendlinje
Dim index As Int32 = chart.NSeries(0).TrendLines.Add(TrendlineType.Linear)
Dim trendline As Trendline = chart.NSeries(0).TrendLines(index)
'Ställa in det anpassade namnet på trendlinjen.
trendline.Name = "Linear"
'Visar ekvationen på diagrammet
trendline.DisplayEquation = True
'Visar R-kvadrat-värdet på diagrammet
trendline.DisplayRSquared = True
'Sparar Excel-filen
workbook.Save("book1.xls")
```

### Se även

* class [Line](../../aspose.cells.drawing/line)
* namnutrymme [Aspose.Cells.Charts](../../aspose.cells.charts)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
