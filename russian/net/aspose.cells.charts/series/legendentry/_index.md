---
title: "Series.LegendEntry"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Получает запись легенды, соответствующую этой серии"
type: docs
url: /ru/net/aspose.cells.charts/series/legendentry/
---
## Series.LegendEntry property

Получает элемент легенды, соответствующий этой серии.

```csharp
public LegendEntry LegendEntry { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyLegendEntryDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить первую серию
            Series series = chart.NSeries[0];

            // Продемонстрировать функциональность LegendEntry
            Console.WriteLine("LegendEntry.IsDeleted before: " + series.LegendEntry.IsDeleted);
            series.LegendEntry.IsDeleted = true;
            Console.WriteLine("LegendEntry.IsDeleted after setting to true: " + series.LegendEntry.IsDeleted);
            series.LegendEntry.IsDeleted = false;
            Console.WriteLine("LegendEntry.IsDeleted after setting to false: " + series.LegendEntry.IsDeleted);

            // Сохраните книгу
            workbook.Save("SeriesPropertyLegendEntryDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [LegendEntry](../../legendentry/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


