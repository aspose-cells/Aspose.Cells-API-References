---
title: "Класс SeriesCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Charts.SeriesCollection класс. Инкапсулирует коллекцию объектов Series."
type: docs
url: /ru/net/aspose.cells.charts/seriescollection/
---
## SeriesCollection class

Инкапсулирует коллекцию объектов [`Series`](../series/).

```csharp
public class SeriesCollection : CollectionBase<Series>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [CategoryData](../../aspose.cells.charts/seriescollection/categorydata/) { get; set; } | Получает или задает диапазон значений оси категорий. Это может быть диапазон ячеек (например, "d1:e10") или последовательность значений (например, "{2,6,8,10}"). |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [IsColorVaried](../../aspose.cells.charts/seriescollection/iscolorvaried/) { get; set; } | Указывает, изменяется ли цвет точек. |
| [Item](../../aspose.cells.charts/seriescollection/item/) { get; } | Получает элемент [`Series`](../series/) по указанному индексу. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [SecondCategoryData](../../aspose.cells.charts/seriescollection/secondcategorydata/) { get; set; } | Получает или задает диапазон значений второй оси категорий. Это может быть диапазон ячеек (например, "d1:e10"), или последовательность значений (например, "{2,6,8,10}"). Действует только когда некоторые серии построены на второй оси. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.charts/seriescollection/add/#add)(string, bool) | Добавляет коллекцию [`Series`](../series/) к диаграмме. |
| [Add](../../aspose.cells.charts/seriescollection/add/#add_1)(string, bool, bool) | Добавляет коллекцию [`Series`](../series/) к диаграмме. |
| [AddR1C1](../../aspose.cells.charts/seriescollection/addr1c1/)(string, bool) | Добавляет коллекцию [`Series`](../series/) к диаграмме. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Series) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Series, IComparer&lt;Series&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Series, IComparer&lt;Series&gt;) |  |
| [ChangeColors](../../aspose.cells.charts/seriescollection/changecolors/)(ChartColorPaletteType) | Установить монохромную палитру для серий диаграммы. |
| [ChangeSeriesOrder](../../aspose.cells.charts/seriescollection/changeseriesorder/)(int, int) | (**Obsolete.**) Непосредственно изменяет порядок двух серий. |
| [Clear](../../aspose.cells.charts/seriescollection/clear/#clear)() | Очищает коллекцию (2 метода) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Series) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Series[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Series[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Series[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Series&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Series&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Series&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Series&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [GetSeriesByOrder](../../aspose.cells.charts/seriescollection/getseriesbyorder/)(int) | Получает элемент [`Series`](../series/) по порядку. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Series) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Series, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Series, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Series) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Series, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Series, int, int) |  |
| [RemoveAt](../../aspose.cells.charts/seriescollection/removeat/#removeat)(int) | Удаляет серию по указанному индексу. (2 метода) |
| [SetSeriesNames](../../aspose.cells.charts/seriescollection/setseriesnames/)(int, string, bool) | Задает имена всех серий в диаграмме. |
| [SwapSeries](../../aspose.cells.charts/seriescollection/swapseries/)(int, int) | Непосредственно изменяет порядок двух серий. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesCollectionDemo
    {
        public static void SeriesCollectionExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            
            // Добавление нового листа к объекту Excel
            int sheetIndex = workbook.Worksheets.Add();
            
            // Получение ссылки на только что добавленный лист путем передачи его индекса листа
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Добавление образцовых значений в ячейки
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Добавление диаграммы в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Получение экземпляра недавно добавленной диаграммы
            Chart chart = worksheet.Charts[chartIndex];
            
            // Добавление NSeries (источник данных диаграммы) к диаграмме, охватывающей ячейки от "A1" до "B4"
            chart.NSeries.Add("A1:B4", true);
            
            // Установка источника данных для категориальных данных NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Доступ к SeriesCollection диаграммы
            SeriesCollection seriesCollection = chart.NSeries;

            // Установка свойств SeriesCollection
            seriesCollection.CategoryData = "C1:C4";
            seriesCollection.SecondCategoryData = "C1:C4";
            seriesCollection.IsColorVaried = true;

            // Доступ к конкретной серии в SeriesCollection
            Series series = seriesCollection[0];
            
            // Установка свойств серии
            series.Values = "=B1:B4";
            series.Name = "First Series";
            series.Type = ChartType.Line;
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.ForegroundColorSetType = FormattingType.Automatic;
            series.Marker.ForegroundColor = System.Drawing.Color.Black;
            series.Marker.BackgroundColorSetType = FormattingType.Automatic;

            // Сохранение файла Excel
            workbook.Save("SeriesCollectionExample.xlsx");
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Series](../series/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


