---
title: Axis
second_title: Aspose.Cells för .NET API-referens
description: Kapslar in objektet som representerar ett diagrams axel.
type: docs
weight: 360
url: /sv/net/aspose.cells.charts/axis/
---
## Axis class

Kapslar in objektet som representerar ett diagrams axel.

```csharp
public class Axis
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Area](../../aspose.cells.charts/axis/area) { get; } | Får[`Area`](./area) . |
| [AxisBetweenCategories](../../aspose.cells.charts/axis/axisbetweencategories) { get; set; } | Representerar om värdeaxeln korsar kategoriaxeln mellan kategorier. |
| [AxisLabels](../../aspose.cells.charts/axis/axislabels) { get; } | Hämtar beteckningarna för axeln efter anropet Chart.Calculate()-metoden. |
| [AxisLine](../../aspose.cells.charts/axis/axisline) { get; } | Får utseendet av en Axis. |
| [BaseUnitScale](../../aspose.cells.charts/axis/baseunitscale) { get; set; } | Representerar basenhetsskalan för kategoriaxeln. |
| [Bins](../../aspose.cells.charts/axis/bins) { get; } | Representerar fack på ett diagram (Histogram/Pareto) axis |
| [CategoryType](../../aspose.cells.charts/axis/categorytype) { get; set; } | Representerar kategoriaxeltypen. |
| [CrossAt](../../aspose.cells.charts/axis/crossat) { get; set; } | Representerar punkten på värdeaxeln där kategoriaxeln korsar den. |
| [CrossType](../../aspose.cells.charts/axis/crosstype) { get; set; } | Representerar[`CrossType`](./crosstype) på den angivna axeln där den andra axeln korsar. |
| [CustUnit](../../aspose.cells.charts/axis/custunit) { get; set; } | Anger ett anpassat värde för visningsenheten. |
| [DisplayUnit](../../aspose.cells.charts/axis/displayunit) { get; set; } | Representerar enhetsetiketten för den angivna axeln. |
| [DisplayUnitLabel](../../aspose.cells.charts/axis/displayunitlabel) { get; } | Representerar en enhetsetikett på en axel i det angivna diagrammet. Enhetsetiketter är användbara för att kartlägga stora värden – till exempel i miljoner eller miljarder. |
| [HasMultiLevelLabels](../../aspose.cells.charts/axis/hasmultilevellabels) { get; set; } | Indikerar om etiketterna ska visas som flernivåer. |
| [IsAutomaticMajorUnit](../../aspose.cells.charts/axis/isautomaticmajorunit) { get; set; } | Indikerar om huvudenheten för axeln tilldelas automatiskt. |
| [IsAutomaticMaxValue](../../aspose.cells.charts/axis/isautomaticmaxvalue) { get; set; } | Indikerar om maxvärdet tilldelas automatiskt. |
| [IsAutomaticMinorUnit](../../aspose.cells.charts/axis/isautomaticminorunit) { get; set; } | Indikerar om axelns mindre enhet tilldelas automatiskt. |
| [IsAutomaticMinValue](../../aspose.cells.charts/axis/isautomaticminvalue) { get; set; } | Indikerar om minvärdet tilldelas automatiskt. |
| [IsAutoTickLabelSpacing](../../aspose.cells.charts/axis/isautoticklabelspacing) { get; set; } | Indikerar om avståndet mellan bocketiketten är automatiskt |
| [IsDisplayUnitLabelShown](../../aspose.cells.charts/axis/isdisplayunitlabelshown) { get; set; } | Representerar om displayenhetens etikett visas på den angivna axeln. |
| [IsLogarithmic](../../aspose.cells.charts/axis/islogarithmic) { get; set; } | Representerar om skaltypen för värdeaxeln är logaritmisk eller inte. |
| [IsPlotOrderReversed](../../aspose.cells.charts/axis/isplotorderreversed) { get; set; } | Representerar om Microsoft Excel plottar datapunkter från sist till första. |
| [IsVisible](../../aspose.cells.charts/axis/isvisible) { get; set; } | Representerar om axeln är synlig. |
| [LogBase](../../aspose.cells.charts/axis/logbase) { get; set; } | Representerar den logaritmiska basen. Standardvärdet är 10. Gäller endast Excel2007. |
| [MajorGridLines](../../aspose.cells.charts/axis/majorgridlines) { get; } | Representerar stora rutnät på en diagramaxel. |
| [MajorTickMark](../../aspose.cells.charts/axis/majortickmark) { get; set; } | Representerar typen av större bock för den angivna axeln. |
| [MajorUnit](../../aspose.cells.charts/axis/majorunit) { get; set; } | Representerar huvudenheterna för axeln. |
| [MajorUnitScale](../../aspose.cells.charts/axis/majorunitscale) { get; set; } | Representerar huvudenhetsskalan för kategoriaxeln. |
| [MaxValue](../../aspose.cells.charts/axis/maxvalue) { get; set; } | Representerar det maximala värdet på värdeaxeln. |
| [MinorGridLines](../../aspose.cells.charts/axis/minorgridlines) { get; } | Representerar mindre rutnät på en diagramaxel. |
| [MinorTickMark](../../aspose.cells.charts/axis/minortickmark) { get; set; } | Representerar typen av mindre bock för den angivna axeln. |
| [MinorUnit](../../aspose.cells.charts/axis/minorunit) { get; set; } | Representerar de mindre enheterna för axeln. |
| [MinorUnitScale](../../aspose.cells.charts/axis/minorunitscale) { get; set; } | Representerar huvudenhetsskalan för kategoriaxeln. |
| [MinValue](../../aspose.cells.charts/axis/minvalue) { get; set; } | Representerar minimivärdet på värdeaxeln. |
| [TickLabelPosition](../../aspose.cells.charts/axis/ticklabelposition) { get; set; } | Representerar positionen för bockmarkeringsetiketter på den angivna axeln. |
| [TickLabels](../../aspose.cells.charts/axis/ticklabels) { get; } | Returnerar en[`TickLabels`](./ticklabels) objekt som representerar tick-mark-etiketterna för den angivna axeln. |
| [TickLabelSpacing](../../aspose.cells.charts/axis/ticklabelspacing) { get; set; } | Representerar antalet kategorier eller serier mellan bockmarkeringsetiketter. Gäller endast kategori- och serieaxlar. |
| [TickMarkSpacing](../../aspose.cells.charts/axis/tickmarkspacing) { get; set; } | Returnerar eller ställer in antalet kategorier eller serier mellan bockmarkeringar. Gäller endast kategori- och serieaxlar. |
| [Title](../../aspose.cells.charts/axis/title) { get; } | Hämtar axelns titel. |

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
//Lägga till ett exempelvärde till "B1"-cellen
worksheet.Cells["B1"].PutValue(4);
//Lägga till ett exempelvärde till "B2"-cellen
worksheet.Cells["B2"].PutValue(20);
//Lägga till ett exempelvärde till "B3"-cellen
worksheet.Cells["B3"].PutValue(50);
//Lägga till ett diagram i arbetsbladet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
//Åtkomst till instansen av det nyligen tillagda diagrammet
Chart chart = worksheet.Charts[chartIndex];
//Lägga till NSeries (diagramdatakälla) till diagrammet som sträcker sig från "A1"-cell till "B3"
chart.NSeries.Add("A1:B3", true);
//Ställ in maxvärdet för värdeaxeln
chart.ValueAxis.MaxValue = 200;
//Ställ in minvärdet för värdeaxeln
chart.ValueAxis.MinValue = 0;
//Ställ in huvudenheten
chart.ValueAxis.MajorUnit = 25;
//Kategori(X)-axeln korsar vid maxinumvärdet.
chart.ValueAxis.CrossType = CrossType.Maximum;
//Ställ in antalet kategorier eller serier mellan bockmarkeringsetiketter. 
chart.CategoryAxis.TickLabelSpacing = 2;

//gör dina affärer

//Spara Excel-filen
workbook.Save("book1.xlsx");

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
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(4)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(20)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'Lägga till ett diagram i arbetsbladet
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5)
'Åtkomst till instansen av det nyligen tillagda diagrammet
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", True)
'Ställ in maxvärdet för värdeaxeln
chart.ValueAxis.MaxValue = 200
'Ställ in minvärdet för värdeaxeln
chart.ValueAxis.MinValue = 0
'Ställ in huvudenheten
chart.ValueAxis.MajorUnit = 25
'Kategori(X)-axeln korsar vid maxinumvärdet.
chart.ValueAxis.CrossType = CrossType.Maximum
'Ställ in antalet kategorier eller serier mellan bockmarkeringsetiketter. 
chart.CategoryAxis.TickLabelSpacing = 2
'Sparar Excel-filen
workbook.Save("book1.xlsx")
```

### Se även

* namnutrymme [Aspose.Cells.Charts](../../aspose.cells.charts)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
