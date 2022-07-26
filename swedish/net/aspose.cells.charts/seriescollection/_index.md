---
title: SeriesCollection
second_title: Aspose.Cells för .NET API-referens
description: Kapslar in en samling avSeries./series objekt.
type: docs
weight: 830
url: /sv/net/aspose.cells.charts/seriescollection/
---
## SeriesCollection class

Kapslar in en samling av[`Series`](../series) objekt.

```csharp
public class SeriesCollection : CollectionBase<Series>
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [CategoryData](../../aspose.cells.charts/seriescollection/categorydata) { get; set; } | Hämtar eller ställer in intervallet för kategoriaxelvärden. Det kan vara ett cellintervall (som "d1:e10"), eller en sekvens av värden (som,"{2,6,8,10}"). |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [IsColorVaried](../../aspose.cells.charts/seriescollection/iscolorvaried) { get; set; } | Representerar om färgen på punkter varieras. |
| [Item](../../aspose.cells.charts/seriescollection/item) { get; } | Får[`Series`](../series) element vid angivet index. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |
| [SecondCategoryData](../../aspose.cells.charts/seriescollection/secondcategorydata) { get; set; } | Hämtar eller ställer in intervallet för andra kategorins axelvärden. Det kan vara ett cellintervall (som "d1:e10"), eller en sekvens av värden (som,"{2,6,8,10}"). Effekter endast när vissa ASeries plottar på den andra axeln. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.charts/seriescollection/add#add)(string, bool) | Lägger till[`SeriesCollection`](../seriescollection) samling till ett diagram. |
| [Add](../../aspose.cells.charts/seriescollection/add#add_1)(string, bool, bool) | Lägger till[`SeriesCollection`](../seriescollection) samling till ett diagram. |
| [AddR1C1](../../aspose.cells.charts/seriescollection/addr1c1)(string, bool) | Lägger till[`SeriesCollection`](../seriescollection) samling till ett diagram. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Series) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Series, IComparer&lt;Series&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Series, IComparer&lt;Series&gt;) |  |
| [ChangeSeriesOrder](../../aspose.cells.charts/seriescollection/changeseriesorder)(int, int) | Ändrar direkt ordningsföljden för de två serierna. |
| [Clear](../../aspose.cells.charts/seriescollection/clear#clear)() | Rensar samlingen (2 methods) |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Series) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Series[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Series[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Series[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Series&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Series&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Series&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Series&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [GetSeriesByOrder](../../aspose.cells.charts/seriescollection/getseriesbyorder)(int) | Får[`Series`](../series) element efter beställning. |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series, int, int) |  |
| [RemoveAt](../../aspose.cells.charts/seriescollection/removeat#removeat)(int) | Ta bort vid en serie vid det specifika indexet. (2 methods) |
| [SetSeriesNames](../../aspose.cells.charts/seriescollection/setseriesnames)(int, string, bool) | Anger namnet på alla serier i diagrammet. |

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
//Spara Excel-filen
workbook.Save("book1.xls");

[Visual Basic]

'Instantiera ett arbetsboksobjekt
Dim workbook As Workbook = New Workbook()
'Lägga till ett nytt kalkylblad till Excel-objektet
Dim sheetIndex As Integer = workbook.Worksheets.Add()
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
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Åtkomst till instansen av det nyligen tillagda diagrammet
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.NSeries.Add("A1:B4", True)
'Ställa in datakällan för kategoridata för NSeries
chart.NSeries.CategoryData = "C1:C4"
'Sparar Excel-filen
workbook.Save("book1.xls")
```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Series](../series)
* namnutrymme [Aspose.Cells.Charts](../../aspose.cells.charts)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
