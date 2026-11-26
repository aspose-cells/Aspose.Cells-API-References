---
title: "Series.HasLeaderLines"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Истина, если у серии есть линии‑выноски"
type: docs
url: /ru/net/aspose.cells.charts/series/hasleaderlines/
---
## Series.HasLeaderLines property

Истина, если у серии есть линии‑выноски.

```csharp
public bool HasLeaderLines { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasLeaderLinesDemo
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

            // Добавить круговую диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Pie, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Включить линии‑выноски для первой серии
            chart.NSeries[0].HasLeaderLines = true;

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


