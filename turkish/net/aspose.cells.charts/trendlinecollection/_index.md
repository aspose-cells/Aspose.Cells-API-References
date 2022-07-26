---
title: TrendlineCollection
second_title: Aspose.Cells for .NET API Referansı
description: Tüm öğelerin bir koleksiyonunu temsil eder.Trendline./trendline belirtilen veri serisi için nesneler.
type: docs
weight: 990
url: /tr/net/aspose.cells.charts/trendlinecollection/
---
## TrendlineCollection class

Tüm öğelerin bir koleksiyonunu temsil eder.[`Trendline`](../trendline) belirtilen veri serisi için nesneler.

```csharp
public class TrendlineCollection : CollectionBase<Trendline>
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.charts/trendlinecollection/item) { get; } | indeksine göre nesne. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Add](../../aspose.cells.charts/trendlinecollection/add#add)(TrendlineType) | Bir ekler belirtilen tür ile bu koleksiyona nesne. |
| [Add](../../aspose.cells.charts/trendlinecollection/add#add_1)(TrendlineType, string) | Bir ekler belirtilen tür ve adla bu koleksiyona nesne. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Trendline) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Trendline, IComparer&lt;Trendline&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Trendline, IComparer&lt;Trendline&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Trendline) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Trendline[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Trendline[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Trendline[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Trendline&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Trendline&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Trendline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Trendline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Trendline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Trendline&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Trendline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Trendline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Trendline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Trendline&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Trendline) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Trendline, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Trendline, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Trendline) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Trendline, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Trendline, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### Örnekler

```csharp
[C#]

//Bir Çalışma Kitabı nesnesini başlatma
Workbook workbook = new Workbook();
//Excel nesnesine yeni bir çalışma sayfası ekleme
int sheetIndex = workbook.Worksheets.Add();
//Yeni eklenen çalışma sayfasının sayfa indeksini geçerek referansının alınması
Worksheet worksheet = workbook.Worksheets[sheetIndex];
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["A4"].PutValue(200);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
worksheet.Cells["B4"].PutValue(40);

//Çalışma sayfasına grafik ekleme
int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 3, 3, 15, 10);
Chart chart = workbook.Worksheets[0].Charts[chartIndex];
chart.NSeries.Add("A1:a3", true);
chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "MyTrendLine");
Trendline line = chart.NSeries[0].TrendLines[0];
line.DisplayEquation = true;
line.DisplayRSquared = true;
line.Color = Color.Red;

[Visual Basic]

'Bir Çalışma Kitabı nesnesini başlatma
Dim workbook As Workbook = New Workbook()
'Excel nesnesine yeni bir çalışma sayfası ekleme
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'Yeni eklenen çalışma sayfasının sayfa indeksini geçerek referansını alma
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
worksheet.Cells("A1").PutValue(50)
worksheet.Cells("A2").PutValue(100)
worksheet.Cells("A3").PutValue(150)
worksheet.Cells("A4").PutValue(200)
worksheet.Cells("B1").PutValue(60)
worksheet.Cells("B2").PutValue(32)
worksheet.Cells("B3").PutValue(50)
worksheet.Cells("B4").PutValue(40)

'Çalışma sayfasına grafik ekleme
Dim chartIndex As Integer =  workbook.Worksheets(0).Charts.Add(ChartType.Column,3,3,15,10) 
Dim chart As Chart =  workbook.Worksheets(0).Charts(chartIndex) 
chart.NSeries.Add("A1:a3", True)
chart.NSeries(0).TrendLines.Add(TrendlineType.Linear, "MyTrendLine")
Dim line As Trendline =  chart.NSeries(0).TrendLines(0) 
line.DisplayEquation = True
line.DisplayRSquared = True
line.Color = Color.Red
```

### Ayrıca bakınız

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Trendline](../trendline)
* ad alanı [Aspose.Cells.Charts](../../aspose.cells.charts)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
