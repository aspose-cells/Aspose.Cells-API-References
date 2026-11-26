---
title: "TrendlineCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TrendlineCollection. Получает объект Trendline по его индексу"
type: docs
url: /ru/net/aspose.cells.charts/trendlinecollection/item/
---
## TrendlineCollection indexer

Получает объект [`Trendline`](../../trendline/) по его индексу.

```csharp
public Trendline this[int index] { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlineCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue(1);
            sheet.Cells["A2"].PutValue(2);
            sheet.Cells["A3"].PutValue(3);
            sheet.Cells["B1"].PutValue(4);
            sheet.Cells["B2"].PutValue(5);
            sheet.Cells["B3"].PutValue(6);

            // Добавьте диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries[0].Values = "B1:B3";

            // Добавить trendline
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];

            // Продемонстрировать использование свойства Item
            Trendline firstTrendline = chart.NSeries[0].TrendLines[0];
            Console.WriteLine("Trendline Type: " + firstTrendline.Type);
        }
    }
}
```

### См. также

* class [Trendline](../../trendline/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


