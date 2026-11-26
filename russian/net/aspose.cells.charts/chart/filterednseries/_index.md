---
title: "Chart.FilteredNSeries"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Получает коллекцию SeriesCollection, представляющую серии данных, отфильтрованные в диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/chart/filterednseries/
---
## Chart.FilteredNSeries property

Получает коллекцию [`SeriesCollection`](../../seriescollection/), представляющую серии данных, отфильтрованные в диаграмме.

```csharp
public SeriesCollection FilteredNSeries { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyFilteredNSeriesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Series");
            worksheet.Cells["A2"].PutValue("Series 1");
            worksheet.Cells["A3"].PutValue("Series 2");
            worksheet.Cells["A4"].PutValue("Series 3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму и установите некоторые серии как отфильтрованные
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Отфильтровать некоторые серии (скрыть Series 2)
            chart.NSeries[1].IsFiltered = true;

            // Получить доступ к коллекции отфильтрованных серий
            Aspose.Cells.Charts.SeriesCollection filteredSeries = chart.FilteredNSeries;
            Console.WriteLine("Filtered Series Count: " + filteredSeries.Count.ToString());

            // Сохраните книгу
            workbook.Save("FilteredNSeriesDemo.xlsx");
        }
    }
}
```

### См. также

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


