---
title: "Класс ChartCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.ChartCollection. Инкапсулирует коллекцию объектов Chart."
type: docs
url: /ru/net/aspose.cells.charts/chartcollection/
---
## ChartCollection class

Инкапсулирует коллекцию объектов [`Chart`](../chart/).

```csharp
public class ChartCollection : CollectionBase<Chart>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.charts/chartcollection/item/) { get; } | Получает элемент [`Chart`](../chart/) по указанному индексу. (2 индексатора) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.charts/chartcollection/add/#add)(ChartType, int, int, int, int) | Добавляет диаграмму в коллекцию. |
| [Add](../../aspose.cells.charts/chartcollection/add/#add_2)(ChartType, string, int, int, int, int) | (**Устарело.**) Добавляет диаграмму в коллекцию. |
| [Add](../../aspose.cells.charts/chartcollection/add/#add_3)(byte[], string, bool, int, int, int, int) | Добавляет диаграмму с предустановленным шаблоном. |
| [Add](../../aspose.cells.charts/chartcollection/add/#add_1)(ChartType, string, bool, int, int, int, int) | Добавляет диаграмму в коллекцию. |
| [AddFloatingChart](../../aspose.cells.charts/chartcollection/addfloatingchart/)(ChartType, int, int, int, int) | Добавляет диаграмму в коллекцию. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Chart) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Chart, IComparer&lt;Chart&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Chart, IComparer&lt;Chart&gt;) |  |
| [Clear](../../aspose.cells.charts/chartcollection/clear/#clear)() | Очистить все диаграммы. (2 метода) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Chart) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Chart[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Chart[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Chart[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Chart&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Chart&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Chart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Chart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Chart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Chart&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Chart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Chart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Chart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Chart&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Chart) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Chart, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Chart, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Chart) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Chart, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Chart, int, int) |  |
| [RemoveAt](../../aspose.cells.charts/chartcollection/removeat/#removeat)(int) | Удалить диаграмму по конкретному индексу. (2 метода) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionDemo
    {
        public static void ChartCollectionExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые образцы данных в лист
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Получить доступ к коллекции диаграмм листа
            ChartCollection charts = worksheet.Charts;

            // Добавить диаграмму в лист
            int chartIndex = charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = charts[chartIndex];

            // Установить диапазон данных для диаграммы
            chart.SetChartDataRange("A1:B4", true);

            // Настроить диаграмму
            chart.Title.Text = "Sample Chart";
            chart.ShowLegend = true;

            // Сохраните книгу
            workbook.Save("ChartCollectionExample.xlsx");
            workbook.Save("ChartCollectionExample.pdf");
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Chart](../chart/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


