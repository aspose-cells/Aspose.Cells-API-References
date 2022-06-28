---
title: SeriesCollection
second_title: Справочник по Aspose.Cells для .NET API
description: Инкапсулирует коллекцию объектовSeries./series.
type: docs
weight: 830
url: /ru/net/aspose.cells.charts/seriescollection/
---
## SeriesCollection class

Инкапсулирует коллекцию объектов[`Series`](../series).

```csharp
public class SeriesCollection : CollectionBase<Series>
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [CategoryData](../../aspose.cells.charts/seriescollection/categorydata) { get; set; } | Получает или задает диапазон значений категории Axis. Это может быть диапазон ячеек (например, "d1:e10"), или последовательность значений (например, "{2,6,8,10 }"). |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [IsColorVaried](../../aspose.cells.charts/seriescollection/iscolorvaried) { get; set; } | Указывает, различаются ли цвета точек. |
| [Item](../../aspose.cells.charts/seriescollection/item) { get; } | Получает элемент[`Series`](../series)по указанному индексу. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |
| [SecondCategoryData](../../aspose.cells.charts/seriescollection/secondcategorydata) { get; set; } | Получает или задает диапазон значений оси второй категории. Это может быть диапазон ячеек (например, "d1:e10"), или последовательность значений (например, "{2,6,8,10 }"). Воздействует только тогда, когда некоторые ASeries строятся по второй оси. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.charts/seriescollection/add#add)(string, bool) | Добавляет коллекцию[`SeriesCollection`](../seriescollection)на диаграмму. |
| [Add](../../aspose.cells.charts/seriescollection/add#add_1)(string, bool, bool) | Добавляет коллекцию[`SeriesCollection`](../seriescollection)на диаграмму. |
| [AddR1C1](../../aspose.cells.charts/seriescollection/addr1c1)(string, bool) | Добавляет коллекцию[`SeriesCollection`](../seriescollection)на диаграмму. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Series) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Series, IComparer&lt;Series&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Series, IComparer&lt;Series&gt;) |  |
| [ChangeSeriesOrder](../../aspose.cells.charts/seriescollection/changeseriesorder)(int, int) | Напрямую изменяет порядок двух рядов. |
| [Clear](../../aspose.cells.charts/seriescollection/clear#clear)() | Очищает коллекцию (2 methods) |
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
| [GetSeriesByOrder](../../aspose.cells.charts/seriescollection/getseriesbyorder)(int) | Получает элемент[`Series`](../series)по порядку. |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series, int, int) |  |
| [RemoveAt](../../aspose.cells.charts/seriescollection/removeat#removeat)(int) | Удалить в серии по определенному индексу. (2 methods) |
| [SetSeriesNames](../../aspose.cells.charts/seriescollection/setseriesnames)(int, string, bool) | Задает имя всех рядов на графике. |

### Примеры

```csharp

[C#]
  //Создание экземпляра рабочей книги object
Workbook workbook = new Workbook();
  //Добавление нового рабочего листа в Excel object
int sheetIndex = workbook.Worksheets.Add();
  //Получение ссылки на вновь добавленный рабочий лист путем передачи его листа index
Worksheet worksheet = workbook.Worksheets[sheetIndex];
  //Добавление значения выборки в "A1" cell
worksheet.Cells["A1"].PutValue(50);
//Добавление значения образца в "A2" cell
worksheet.Cells["A2"].PutValue(100);
  //Добавление значения образца в "A3" cell
worksheet.Cells["A3"].PutValue(150);
  //Добавление образца значения в "A4" cell
worksheet.Cells["A4"].PutValue(200);
  //Добавление образца значения в "B1" cell
worksheet.Cells["B1"].PutValue(60);
  //Добавление значения образца в "B2" cell
worksheet.Cells["B2"].PutValue(32);
  //Добавление значения образца в "B3" cell
worksheet.Cells["B3"].PutValue(50);
  //Добавление значения образца в "B4" cell
worksheet.Cells["B4"].PutValue(40);
  //Добавление образца значения в ячейку "C1" как категория data
worksheet.Cells["C1"].PutValue("Q1");
  //Добавление образца значения в ячейку "C2" как категория data
worksheet.Cells["C2"].PutValue("Q2");
  //Добавление значения образца в ячейку "C3" как категория data
worksheet.Cells["C3"].PutValue("Y1");
  //Добавление образца значения в ячейку "C4" как категория data
worksheet.Cells["C4"].PutValue("Y2");
  //Добавление диаграммы на лист
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
  //Доступ к экземпляру только что добавленного chart
Chart chart = worksheet.Charts[chartIndex];
  //Добавление NSeries (источника данных диаграммы) на диаграмму в диапазоне от ячейки "A1" до "B4"
chart.NSeries.Add("A1:B4", true);
  //Установка источника данных для данных категории NSeries
chart.NSeries.CategoryData = "C1:C4";
  //Сохранение файла Excel
workbook.Save("book1.xls");

[Visual Basic]

'Создание экземпляра рабочей книги object
Dim workbook As Workbook = New Workbook()
'Добавление нового рабочего листа в Excel object
Dim sheetIndex As Integer = workbook.Worksheets.Add()
'Получение ссылки на вновь добавленный рабочий лист путем передачи его листа index
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Добавление значения выборки в "A1" cell
worksheet.Cells("A1").PutValue(50)
'Добавление значения выборки в "A2" cell
worksheet.Cells("A2").PutValue(100)
'Добавление значения выборки в "A3" cell
worksheet.Cells("A3").PutValue(150)
'Добавление значения выборки в "A4" cell
worksheet.Cells("A4").PutValue(200)
'Добавление образца значения в "B1" cell
worksheet.Cells("B1").PutValue(60)
'Добавление образца значения в "B2 cell
worksheet.Cells("B2").PutValue(32)
'Добавление образца значения в "B3" cell
worksheet.Cells("B3").PutValue(50)
'Добавление образца значения в "B4" cell
worksheet.Cells("B4").PutValue(40)
'Добавление образца значения в ячейку "C1" как категория data
worksheet.Cells("C1").PutValue("Q1")
'Добавление образца значения в ячейку "C2" как категория data
worksheet.Cells("C2").PutValue("Q2")
'Добавление образца значения в ячейку "C3" как категория data
worksheet.Cells("C3").PutValue("Y1")
'Добавление образца значения в ячейку "C4" как категория data
worksheet.Cells("C4").PutValue("Y2")
'Добавление диаграммы на лист
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Доступ к экземпляру только что добавленного chart
Dim chart As Chart = worksheet.Charts(chartIndex)
'Добавление NSeries (источника данных диаграммы) на диаграмму в диапазоне от ячейки "A1" до "B4"
chart.NSeries.Add("A1:B4", True)
'Установка источника данных для данных категории NSeries
chart.NSeries.CategoryData = "C1:C4"
'Сохранение файла Excel
workbook.Save("book1.xls")
```

### Смотрите также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Series](../series)
* пространство имен [Aspose.Cells.Charts](../../aspose.cells.charts)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
