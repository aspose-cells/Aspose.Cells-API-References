---
title: SeriesCollection
second_title: Aspose.Cells for .NET API Referansı
description: Bir koleksiyonu kapsüllerSeries./series nesneler.
type: docs
weight: 830
url: /tr/net/aspose.cells.charts/seriescollection/
---
## SeriesCollection class

Bir koleksiyonu kapsüller[`Series`](../series) nesneler.

```csharp
public class SeriesCollection : CollectionBase<Series>
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [CategoryData](../../aspose.cells.charts/seriescollection/categorydata) { get; set; } | Kategori Eksen değerlerinin aralığını alır veya ayarlar. Bir hücre aralığı ("d1:e10" gibi), veya bir değer dizisi ("{2,6,8,10}" gibi) olabilir. |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [IsColorVaried](../../aspose.cells.charts/seriescollection/iscolorvaried) { get; set; } | Noktaların renginin değişip değişmediğini temsil eder. |
| [Item](../../aspose.cells.charts/seriescollection/item) { get; } | [`Series`](../series) belirtilen dizindeki öğe. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |
| [SecondCategoryData](../../aspose.cells.charts/seriescollection/secondcategorydata) { get; set; } | İkinci kategori Eksen değerlerinin aralığını alır veya ayarlar. Bir hücre aralığı ("d1:e10" gibi), veya bir değer dizisi ("{2,6,8,10}" gibi) olabilir. Yalnızca bazı ASeriler ikinci eksende çizim yaptığında etkiler. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Add](../../aspose.cells.charts/seriescollection/add#add)(string, bool) | [`SeriesCollection`](../seriescollection) bir grafiğe toplama. |
| [Add](../../aspose.cells.charts/seriescollection/add#add_1)(string, bool, bool) | [`SeriesCollection`](../seriescollection) bir grafiğe toplama. |
| [AddR1C1](../../aspose.cells.charts/seriescollection/addr1c1)(string, bool) | [`SeriesCollection`](../seriescollection) bir grafiğe toplama. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Series) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Series, IComparer&lt;Series&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Series, IComparer&lt;Series&gt;) |  |
| [ChangeSeriesOrder](../../aspose.cells.charts/seriescollection/changeseriesorder)(int, int) | İki serinin sırasını doğrudan değiştirir. |
| [Clear](../../aspose.cells.charts/seriescollection/clear#clear)() | Koleksiyonu temizler (2 methods) |
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
| [GetSeriesByOrder](../../aspose.cells.charts/seriescollection/getseriesbyorder)(int) | [`Series`](../series) siparişe göre öğe. |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series, int, int) |  |
| [RemoveAt](../../aspose.cells.charts/seriescollection/removeat#removeat)(int) | Belirli dizindeki bir dizide kaldırın. (2 methods) |
| [SetSeriesNames](../../aspose.cells.charts/seriescollection/setseriesnames)(int, string, bool) | Grafikteki tüm serilerin adını belirler. |

### Örnekler

```csharp

[C#]
//Bir Çalışma Kitabı nesnesini başlatma
Workbook workbook = new Workbook();
//Excel nesnesine yeni bir çalışma sayfası ekleme
int sheetIndex = workbook.Worksheets.Add();
//Yeni eklenen çalışma sayfasının sayfa indeksini geçerek referansının alınması
Worksheet worksheet = workbook.Worksheets[sheetIndex];
//"A1" hücresine örnek değer ekleme
worksheet.Cells["A1"].PutValue(50);
//"A2" hücresine örnek değer ekleme
worksheet.Cells["A2"].PutValue(100);
//"A3" hücresine örnek değer ekleme
worksheet.Cells["A3"].PutValue(150);
//"A4" hücresine örnek değer ekleme
worksheet.Cells["A4"].PutValue(200);
//"B1" hücresine örnek değer ekleme
worksheet.Cells["B1"].PutValue(60);
//"B2" hücresine örnek değer ekleme
worksheet.Cells["B2"].PutValue(32);
//"B3" hücresine örnek değer ekleme
worksheet.Cells["B3"].PutValue(50);
//"B4" hücresine örnek değer ekleme
worksheet.Cells["B4"].PutValue(40);
//"C1" hücresine kategori verisi olarak örnek değer ekleme
worksheet.Cells["C1"].PutValue("Q1");
//"C2" hücresine kategori verisi olarak örnek değer ekleme
worksheet.Cells["C2"].PutValue("Q2");
//"C3" hücresine kategori verisi olarak örnek değer ekleme
worksheet.Cells["C3"].PutValue("Y1");
//"C4" hücresine kategori verisi olarak örnek değer ekleme
worksheet.Cells["C4"].PutValue("Y2");
//Çalışma sayfasına grafik ekleme
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
//Yeni eklenen grafiğin örneğine erişim
Chart chart = worksheet.Charts[chartIndex];
//"A1" hücresinden "B4"e kadar olan grafiğe NSeries (grafik veri kaynağı) ekleme
chart.NSeries.Add("A1:B4", true);
// NSeries'in kategori verileri için veri kaynağının ayarlanması
chart.NSeries.CategoryData = "C1:C4";
//Excel dosyasını kaydetme
workbook.Save("book1.xls");

[Visual Basic]

'Bir Çalışma Kitabı nesnesini başlatma
Dim workbook As Workbook = New Workbook()
'Excel nesnesine yeni bir çalışma sayfası ekleme
Dim sheetIndex As Integer = workbook.Worksheets.Add()
'Yeni eklenen çalışma sayfasının sayfa indeksini geçerek referansını alma
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
'Çalışma sayfasına grafik ekleme
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Yeni eklenen grafiğin örneğine erişme
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.NSeries.Add("A1:B4", True)
'NSeries kategori verileri için veri kaynağını ayarlama
chart.NSeries.CategoryData = "C1:C4"
'Excel dosyasını kaydetme
workbook.Save("book1.xls")
```

### Ayrıca bakınız

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Series](../series)
* ad alanı [Aspose.Cells.Charts](../../aspose.cells.charts)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
