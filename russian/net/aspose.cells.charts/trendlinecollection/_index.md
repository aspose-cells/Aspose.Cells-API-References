---
title: TrendlineCollection
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет набор всех объектовTrendline./trendlineдля указанного ряда данных.
type: docs
weight: 990
url: /ru/net/aspose.cells.charts/trendlinecollection/
---
## TrendlineCollection class

Представляет набор всех объектов[`Trendline`](../trendline)для указанного ряда данных.

```csharp
public class TrendlineCollection : CollectionBase<Trendline>
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.charts/trendlinecollection/item) { get; } | Получает объектпо его индексу. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.charts/trendlinecollection/add#add)(TrendlineType) | Добавляет в эту коллекцию объектуказанного типа. |
| [Add](../../aspose.cells.charts/trendlinecollection/add#add_1)(TrendlineType, string) | Добавляет в эту коллекцию объектс указанным типом и именем. |
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

### Примеры

```csharp
[C#]

  //Создание экземпляра рабочей книги object
Workbook workbook = new Workbook();
  //Добавление нового рабочего листа в Excel object
int sheetIndex = workbook.Worksheets.Add();
  //Получение ссылки на вновь добавленный рабочий лист путем передачи его листа index
Worksheet worksheet = workbook.Worksheets[sheetIndex];
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["A4"].PutValue(200);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
worksheet.Cells["B4"].PutValue(40);

  //Добавление диаграммы на лист
int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 3, 3, 15, 10);
Chart chart = workbook.Worksheets[0].Charts[chartIndex];
chart.NSeries.Add("A1:a3", true);
chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "MyTrendLine");
Trendline line = chart.NSeries[0].TrendLines[0];
line.DisplayEquation = true;
line.DisplayRSquared = true;
line.Color = Color.Red;

[Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Adding a new worksheet to the Excel object
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'Obtaining the reference of the newly added worksheet by passing its sheet index
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
worksheet.Cells("A1").PutValue(50)
worksheet.Cells("A2").PutValue(100)
worksheet.Cells("A3").PutValue(150)
worksheet.Cells("A4").PutValue(200)
worksheet.Cells("B1").PutValue(60)
worksheet.Cells("B2").PutValue(32)
worksheet.Cells("B3").PutValue(50)
worksheet.Cells("B4").PutValue(40)

'Adding a chart to the worksheet
Dim chartIndex As Integer =  workbook.Worksheets(0).Charts.Add(ChartType.Column,3,3,15,10) 
Dim chart As Chart =  workbook.Worksheets(0).Charts(chartIndex) 
chart.NSeries.Add("A1:a3", True)
chart.NSeries(0).TrendLines.Add(TrendlineType.Linear, "MyTrendLine")
Dim line As Trendline =  chart.NSeries(0).TrendLines(0) 
line.DisplayEquation = True
line.DisplayRSquared = True
line.Color = Color.Red
```

### Смотрите также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Trendline](../trendline)
* пространство имен [Aspose.Cells.Charts](../../aspose.cells.charts)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
